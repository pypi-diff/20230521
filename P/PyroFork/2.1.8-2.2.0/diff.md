# Comparing `tmp/PyroFork-2.1.8.tar.gz` & `tmp/PyroFork-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyroFork-2.1.8.tar", last modified: Wed May 17 11:33:09 2023, max compression
+gzip compressed data, was "PyroFork-2.2.0.tar", last modified: Sun May 21 13:38:06 2023, max compression
```

## Comparing `PyroFork-2.1.8.tar` & `PyroFork-2.2.0.tar`

### file list

```diff
@@ -1,523 +1,523 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.722386 PyroFork-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-17 11:32:54.000000 PyroFork-2.1.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-17 11:32:54.000000 PyroFork-2.1.8/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-17 11:32:54.000000 PyroFork-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-17 11:32:54.000000 PyroFork-2.1.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-17 11:33:09.722386 PyroFork-2.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.662385 PyroFork-2.1.8/PyroFork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-17 11:33:09.000000 PyroFork-2.1.8/PyroFork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-05-17 11:33:09.000000 PyroFork-2.1.8/PyroFork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:33:09.000000 PyroFork-2.1.8/PyroFork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:33:09.000000 PyroFork-2.1.8/PyroFork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 11:33:09.000000 PyroFork-2.1.8/PyroFork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 11:33:09.000000 PyroFork-2.1.8/PyroFork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-17 11:32:54.000000 PyroFork-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.662385 PyroFork-2.1.8/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.662385 PyroFork-2.1.8/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.662385 PyroFork-2.1.8/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (123)   169763 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.662385 PyroFork-2.1.8/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.662385 PyroFork-2.1.8/compiler/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20053 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/docs/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.662385 PyroFork-2.1.8/compiler/docs/template/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/docs/template/page.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.662385 PyroFork-2.1.8/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.662385 PyroFork-2.1.8/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.662385 PyroFork-2.1.8/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 11:32:54.000000 PyroFork-2.1.8/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.666385 PyroFork-2.1.8/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40779 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.666385 PyroFork-2.1.8/pyrogram/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.666385 PyroFork-2.1.8/pyrogram/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.666385 PyroFork-2.1.8/pyrogram/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.666385 PyroFork-2.1.8/pyrogram/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.670385 PyroFork-2.1.8/pyrogram/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.670385 PyroFork-2.1.8/pyrogram/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.670385 PyroFork-2.1.8/pyrogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.670385 PyroFork-2.1.8/pyrogram/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.670385 PyroFork-2.1.8/pyrogram/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.674385 PyroFork-2.1.8/pyrogram/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.678385 PyroFork-2.1.8/pyrogram/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.682385 PyroFork-2.1.8/pyrogram/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.686385 PyroFork-2.1.8/pyrogram/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.686385 PyroFork-2.1.8/pyrogram/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.690385 PyroFork-2.1.8/pyrogram/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.694385 PyroFork-2.1.8/pyrogram/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/messages/vote_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.694385 PyroFork-2.1.8/pyrogram/methods/password/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.698385 PyroFork-2.1.8/pyrogram/methods/stickers/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/stickers/get_sticker_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.698385 PyroFork-2.1.8/pyrogram/methods/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/users/update_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.698385 PyroFork-2.1.8/pyrogram/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.698385 PyroFork-2.1.8/pyrogram/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.698385 PyroFork-2.1.8/pyrogram/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.702385 PyroFork-2.1.8/pyrogram/raw/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.702385 PyroFork-2.1.8/pyrogram/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.702385 PyroFork-2.1.8/pyrogram/session/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.702385 PyroFork-2.1.8/pyrogram/session/internals/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.702385 PyroFork-2.1.8/pyrogram/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/storage/mongo_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.706385 PyroFork-2.1.8/pyrogram/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.706385 PyroFork-2.1.8/pyrogram/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.710385 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.710385 PyroFork-2.1.8/pyrogram/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.714385 PyroFork-2.1.8/pyrogram/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.714385 PyroFork-2.1.8/pyrogram/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.718386 PyroFork-2.1.8/pyrogram/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (123)   153174 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.722386 PyroFork-2.1.8/pyrogram/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-17 11:32:54.000000 PyroFork-2.1.8/pyrogram/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 11:32:54.000000 PyroFork-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 11:33:09.722386 PyroFork-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-17 11:32:54.000000 PyroFork-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.722386 PyroFork-2.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 11:32:54.000000 PyroFork-2.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.722386 PyroFork-2.1.8/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-17 11:32:54.000000 PyroFork-2.1.8/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-17 11:32:54.000000 PyroFork-2.1.8/tests/filters/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.722386 PyroFork-2.1.8/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 11:32:54.000000 PyroFork-2.1.8/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-17 11:32:54.000000 PyroFork-2.1.8/tests/parser/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-17 11:32:54.000000 PyroFork-2.1.8/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.931979 PyroFork-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-21 13:37:50.000000 PyroFork-2.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-21 13:37:50.000000 PyroFork-2.2.0/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-21 13:37:50.000000 PyroFork-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-21 13:37:50.000000 PyroFork-2.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-21 13:38:06.931979 PyroFork-2.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.867977 PyroFork-2.2.0/PyroFork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-21 13:38:06.000000 PyroFork-2.2.0/PyroFork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-05-21 13:38:06.000000 PyroFork-2.2.0/PyroFork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:38:06.000000 PyroFork-2.2.0/PyroFork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:38:06.000000 PyroFork-2.2.0/PyroFork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-21 13:38:06.000000 PyroFork-2.2.0/PyroFork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 13:38:06.000000 PyroFork-2.2.0/PyroFork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-21 13:37:50.000000 PyroFork-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.867977 PyroFork-2.2.0/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.867977 PyroFork-2.2.0/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.867977 PyroFork-2.2.0/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (123)   169763 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.867977 PyroFork-2.2.0/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.871977 PyroFork-2.2.0/compiler/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20053 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/docs/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.871977 PyroFork-2.2.0/compiler/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/docs/template/page.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.871977 PyroFork-2.2.0/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.871977 PyroFork-2.2.0/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.871977 PyroFork-2.2.0/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-21 13:37:50.000000 PyroFork-2.2.0/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.871977 PyroFork-2.2.0/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40764 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.875978 PyroFork-2.2.0/pyrogram/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.875978 PyroFork-2.2.0/pyrogram/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.875978 PyroFork-2.2.0/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.875978 PyroFork-2.2.0/pyrogram/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.879978 PyroFork-2.2.0/pyrogram/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.879978 PyroFork-2.2.0/pyrogram/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.879978 PyroFork-2.2.0/pyrogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.879978 PyroFork-2.2.0/pyrogram/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.879978 PyroFork-2.2.0/pyrogram/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.883978 PyroFork-2.2.0/pyrogram/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.883978 PyroFork-2.2.0/pyrogram/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.891978 PyroFork-2.2.0/pyrogram/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.891978 PyroFork-2.2.0/pyrogram/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.895978 PyroFork-2.2.0/pyrogram/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.895978 PyroFork-2.2.0/pyrogram/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.903978 PyroFork-2.2.0/pyrogram/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/messages/vote_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.903978 PyroFork-2.2.0/pyrogram/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.903978 PyroFork-2.2.0/pyrogram/methods/stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/stickers/get_sticker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.907978 PyroFork-2.2.0/pyrogram/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.907978 PyroFork-2.2.0/pyrogram/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.907978 PyroFork-2.2.0/pyrogram/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.907978 PyroFork-2.2.0/pyrogram/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.911979 PyroFork-2.2.0/pyrogram/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.911979 PyroFork-2.2.0/pyrogram/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.911979 PyroFork-2.2.0/pyrogram/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.911979 PyroFork-2.2.0/pyrogram/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.911979 PyroFork-2.2.0/pyrogram/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/storage/mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.911979 PyroFork-2.2.0/pyrogram/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.911979 PyroFork-2.2.0/pyrogram/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.915979 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.919979 PyroFork-2.2.0/pyrogram/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.919979 PyroFork-2.2.0/pyrogram/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.919979 PyroFork-2.2.0/pyrogram/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.923979 PyroFork-2.2.0/pyrogram/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153586 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.927979 PyroFork-2.2.0/pyrogram/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-21 13:37:50.000000 PyroFork-2.2.0/pyrogram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-21 13:37:50.000000 PyroFork-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 13:38:06.931979 PyroFork-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-21 13:37:50.000000 PyroFork-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.927979 PyroFork-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-21 13:37:50.000000 PyroFork-2.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.931979 PyroFork-2.2.0/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-21 13:37:50.000000 PyroFork-2.2.0/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-21 13:37:50.000000 PyroFork-2.2.0/tests/filters/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:38:06.931979 PyroFork-2.2.0/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-21 13:37:50.000000 PyroFork-2.2.0/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-21 13:37:50.000000 PyroFork-2.2.0/tests/parser/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-21 13:37:50.000000 PyroFork-2.2.0/tests/test_file_id.py
```

### Comparing `PyroFork-2.1.8/COPYING` & `PyroFork-2.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/COPYING.lesser` & `PyroFork-2.2.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/NOTICE` & `PyroFork-2.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/PKG-INFO` & `PyroFork-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork
-Version: 2.1.8
+Version: 2.2.0
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest
 Author: wulan17
 Author-email: mayuri@mayuri.my.id
 License: LGPLv3
 Project-URL: Tracker, https://github.com/Mayuri-Chan/pyrofork/issues
@@ -14,29 +14,27 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: ~=3.7
+Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 <p align="center">
     <a href="https://github.com/Mayuri-Chan/pyrofork">
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: PyroFork Version: 2.1.8 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: PyroFork Version: 2.2.0 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork Download-URL: https://
 github.com/Mayuri-Chan/pyrofork/releases/latest Author: wulan17 Author-email:
 mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker, https://github.com/
 Mayuri-Chan/pyrofork/issues Project-URL: Source, https://github.com/Mayuri-
 Chan/pyrofork Project-URL: Documentation, https://pyrofork.mayuri.my.id
 Keywords: telegram chat messenger mtproto api client library python Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: Implementation Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet
-Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Software Development :: Libraries :: Application Frameworks Requires-Python:
-~=3.7 Description-Content-Type: text/markdown License-File: COPYING License-
-File: COPYING.lesser License-File: NOTICE
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: Implementation Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Internet Classifier: Topic ::
+Communications Classifier: Topic :: Communications :: Chat Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Topic :: Software Development ::
+Libraries :: Application Frameworks Requires-Python: ~=3.9 Description-Content-
+Type: text/markdown License-File: COPYING License-File: COPYING.lesser License-
+File: NOTICE
                                   [PyroFork]
                   Telegram MTProto API Framework for Python
                           Homepage â¢ Documentation
 ## PyroFork > Elegant, modern and asynchronous Telegram MTProto API framework
 in Python for users and bots ``` python from pyrogram import Client, filters
 app = Client("my_account") @app.on_message(filters.private) async def hello
 (client, message): await message.reply("Hello from Pyrogram!") app.run() ```
```

### Comparing `PyroFork-2.1.8/PyroFork.egg-info/PKG-INFO` & `PyroFork-2.2.0/PyroFork.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork
-Version: 2.1.8
+Version: 2.2.0
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest
 Author: wulan17
 Author-email: mayuri@mayuri.my.id
 License: LGPLv3
 Project-URL: Tracker, https://github.com/Mayuri-Chan/pyrofork/issues
@@ -14,29 +14,27 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: ~=3.7
+Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 <p align="center">
     <a href="https://github.com/Mayuri-Chan/pyrofork">
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: PyroFork Version: 2.1.8 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: PyroFork Version: 2.2.0 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork Download-URL: https://
 github.com/Mayuri-Chan/pyrofork/releases/latest Author: wulan17 Author-email:
 mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker, https://github.com/
 Mayuri-Chan/pyrofork/issues Project-URL: Source, https://github.com/Mayuri-
 Chan/pyrofork Project-URL: Documentation, https://pyrofork.mayuri.my.id
 Keywords: telegram chat messenger mtproto api client library python Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: Implementation Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet
-Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Software Development :: Libraries :: Application Frameworks Requires-Python:
-~=3.7 Description-Content-Type: text/markdown License-File: COPYING License-
-File: COPYING.lesser License-File: NOTICE
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: Implementation Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Internet Classifier: Topic ::
+Communications Classifier: Topic :: Communications :: Chat Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Topic :: Software Development ::
+Libraries :: Application Frameworks Requires-Python: ~=3.9 Description-Content-
+Type: text/markdown License-File: COPYING License-File: COPYING.lesser License-
+File: NOTICE
                                   [PyroFork]
                   Telegram MTProto API Framework for Python
                           Homepage â¢ Documentation
 ## PyroFork > Elegant, modern and asynchronous Telegram MTProto API framework
 in Python for users and bots ``` python from pyrogram import Client, filters
 app = Client("my_account") @app.on_message(filters.private) async def hello
 (client, message): await message.reply("Hello from Pyrogram!") app.run() ```
```

### Comparing `PyroFork-2.1.8/PyroFork.egg-info/SOURCES.txt` & `PyroFork-2.2.0/PyroFork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/README.md` & `PyroFork-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/__init__.py` & `PyroFork-2.2.0/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/api/__init__.py` & `PyroFork-2.2.0/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/api/compiler.py` & `PyroFork-2.2.0/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/api/source/auth_key.tl` & `PyroFork-2.2.0/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/api/source/main_api.tl` & `PyroFork-2.2.0/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/api/source/sys_msgs.tl` & `PyroFork-2.2.0/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/api/template/combinator.txt` & `PyroFork-2.2.0/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/api/template/type.txt` & `PyroFork-2.2.0/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/docs/__init__.py` & `PyroFork-2.2.0/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/docs/compiler.py` & `PyroFork-2.2.0/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/errors/__init__.py` & `PyroFork-2.2.0/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/errors/compiler.py` & `PyroFork-2.2.0/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/errors/sort.py` & `PyroFork-2.2.0/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/errors/source/400_BAD_REQUEST.tsv` & `PyroFork-2.2.0/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/errors/source/401_UNAUTHORIZED.tsv` & `PyroFork-2.2.0/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/errors/source/403_FORBIDDEN.tsv` & `PyroFork-2.2.0/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `PyroFork-2.2.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `PyroFork-2.2.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/__init__.py` & `PyroFork-2.2.0/pyrogram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "PyroFork"
-__version__ = "2.1.8"
+__version__ = "2.2.0"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `PyroFork-2.1.8/pyrogram/client.py` & `PyroFork-2.2.0/pyrogram/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             Pass True to start an in-memory session that will be discarded as soon as the client stops.
             In order to reconnect again using an in-memory session without having to login again, you can use
             :meth:`~pyrogram.Client.export_session_string` before stopping the client to get a session string you can
             pass to the ``session_string`` parameter.
             Defaults to False.
 
         mongodb (``dict``, *optional*):
-            Mongodb config as dict, e.g.: *dict(uri="mongodb://...", db_name="pyrofork-session", remove_peers=False)*.
+            Mongodb config as dict, e.g.: *dict(uri="mongodb://...", remove_peers=False)*.
             Only applicable for new sessions.
 
         phone_number (``str``, *optional*):
             Pass the phone number as string (with the Country Code prefix included) to avoid entering it manually.
             Only applicable for new sessions.
 
         phone_code (``str``, *optional*):
@@ -251,15 +251,15 @@
         self.executor = ThreadPoolExecutor(self.workers, thread_name_prefix="Handler")
 
         if self.session_string:
             self.storage = MemoryStorage(self.name, self.session_string)
         elif self.in_memory:
             self.storage = MemoryStorage(self.name)
         elif self.mongodb:
-            self.storage = MongoStorage(self.mongodb)
+            self.storage = MongoStorage(self.name, **self.mongodb)
         else:
             self.storage = FileStorage(self.name, self.workdir)
 
         self.dispatcher = Dispatcher(self)
 
         self.rnd_id = MsgId
```

### Comparing `PyroFork-2.1.8/pyrogram/connection/__init__.py` & `PyroFork-2.2.0/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/connection/connection.py` & `PyroFork-2.2.0/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/connection/transport/__init__.py` & `PyroFork-2.2.0/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/connection/transport/tcp/__init__.py` & `PyroFork-2.2.0/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp.py` & `PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp_abridged.py` & `PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp_full.py` & `PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `PyroFork-2.2.0/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/crypto/__init__.py` & `PyroFork-2.2.0/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/crypto/aes.py` & `PyroFork-2.2.0/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/crypto/mtproto.py` & `PyroFork-2.2.0/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/crypto/prime.py` & `PyroFork-2.2.0/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/crypto/rsa.py` & `PyroFork-2.2.0/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/dispatcher.py` & `PyroFork-2.2.0/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/emoji.py` & `PyroFork-2.2.0/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/__init__.py` & `PyroFork-2.2.0/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/auto_name.py` & `PyroFork-2.2.0/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/chat_action.py` & `PyroFork-2.2.0/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/chat_event_action.py` & `PyroFork-2.2.0/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/chat_member_status.py` & `PyroFork-2.2.0/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/chat_members_filter.py` & `PyroFork-2.2.0/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/chat_type.py` & `PyroFork-2.2.0/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/message_entity_type.py` & `PyroFork-2.2.0/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/message_media_type.py` & `PyroFork-2.2.0/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/message_service_type.py` & `PyroFork-2.2.0/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/messages_filter.py` & `PyroFork-2.2.0/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/next_code_type.py` & `PyroFork-2.2.0/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/parse_mode.py` & `PyroFork-2.2.0/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/poll_type.py` & `PyroFork-2.2.0/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/sent_code_type.py` & `PyroFork-2.2.0/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/enums/user_status.py` & `PyroFork-2.2.0/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/errors/__init__.py` & `PyroFork-2.2.0/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/errors/rpc_error.py` & `PyroFork-2.2.0/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/file_id.py` & `PyroFork-2.2.0/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/filters.py` & `PyroFork-2.2.0/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/__init__.py` & `PyroFork-2.2.0/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/callback_query_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/chat_join_request_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/chat_member_updated_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/chosen_inline_result_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/deleted_messages_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/disconnect_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/edited_message_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/handler.py` & `PyroFork-2.2.0/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/inline_query_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/message_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/poll_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/raw_update_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/handlers/user_status_handler.py` & `PyroFork-2.2.0/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/advanced/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/advanced/invoke.py` & `PyroFork-2.2.0/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/advanced/resolve_peer.py` & `PyroFork-2.2.0/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/advanced/save_file.py` & `PyroFork-2.2.0/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/accept_terms_of_service.py` & `PyroFork-2.2.0/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/check_password.py` & `PyroFork-2.2.0/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/connect.py` & `PyroFork-2.2.0/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/disconnect.py` & `PyroFork-2.2.0/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/get_password_hint.py` & `PyroFork-2.2.0/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/initialize.py` & `PyroFork-2.2.0/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/log_out.py` & `PyroFork-2.2.0/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/recover_password.py` & `PyroFork-2.2.0/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/resend_code.py` & `PyroFork-2.2.0/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/send_code.py` & `PyroFork-2.2.0/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/send_recovery_code.py` & `PyroFork-2.2.0/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/sign_in.py` & `PyroFork-2.2.0/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/sign_in_bot.py` & `PyroFork-2.2.0/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/sign_up.py` & `PyroFork-2.2.0/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/auth/terminate.py` & `PyroFork-2.2.0/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/answer_callback_query.py` & `PyroFork-2.2.0/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/answer_inline_query.py` & `PyroFork-2.2.0/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/answer_web_app_query.py` & `PyroFork-2.2.0/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/delete_bot_commands.py` & `PyroFork-2.2.0/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/get_bot_commands.py` & `PyroFork-2.2.0/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/get_bot_default_privileges.py` & `PyroFork-2.2.0/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/get_chat_menu_button.py` & `PyroFork-2.2.0/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/get_game_high_scores.py` & `PyroFork-2.2.0/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/get_inline_bot_results.py` & `PyroFork-2.2.0/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/request_callback_answer.py` & `PyroFork-2.2.0/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/send_game.py` & `PyroFork-2.2.0/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/send_inline_bot_result.py` & `PyroFork-2.2.0/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/set_bot_commands.py` & `PyroFork-2.2.0/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/set_bot_default_privileges.py` & `PyroFork-2.2.0/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/set_chat_menu_button.py` & `PyroFork-2.2.0/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/bots/set_game_score.py` & `PyroFork-2.2.0/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/add_chat_members.py` & `PyroFork-2.2.0/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/archive_chats.py` & `PyroFork-2.2.0/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/ban_chat_member.py` & `PyroFork-2.2.0/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/close_forum_topic.py` & `PyroFork-2.2.0/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/close_general_topic.py` & `PyroFork-2.2.0/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/create_channel.py` & `PyroFork-2.2.0/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/create_forum_topic.py` & `PyroFork-2.2.0/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/create_group.py` & `PyroFork-2.2.0/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/create_supergroup.py` & `PyroFork-2.2.0/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/delete_channel.py` & `PyroFork-2.2.0/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/delete_chat_photo.py` & `PyroFork-2.2.0/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/delete_forum_topic.py` & `PyroFork-2.2.0/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/delete_supergroup.py` & `PyroFork-2.2.0/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/delete_user_history.py` & `PyroFork-2.2.0/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/edit_forum_topic.py` & `PyroFork-2.2.0/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/edit_general_topic.py` & `PyroFork-2.2.0/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_chat.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_chat_event_log.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_chat_member.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_chat_members.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_chat_members_count.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_chat_online_count.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_dialogs.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_dialogs_count.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_forum_topics.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_forum_topics_by_id.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_nearby_chats.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/get_send_as_chats.py` & `PyroFork-2.2.0/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/hide_general_topic.py` & `PyroFork-2.2.0/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/join_chat.py` & `PyroFork-2.2.0/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/leave_chat.py` & `PyroFork-2.2.0/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/mark_chat_unread.py` & `PyroFork-2.2.0/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/pin_chat_message.py` & `PyroFork-2.2.0/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/promote_chat_member.py` & `PyroFork-2.2.0/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/reopen_forum_topic.py` & `PyroFork-2.2.0/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/reopen_general_topic.py` & `PyroFork-2.2.0/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/restrict_chat_member.py` & `PyroFork-2.2.0/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/set_administrator_title.py` & `PyroFork-2.2.0/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/set_chat_description.py` & `PyroFork-2.2.0/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/set_chat_permissions.py` & `PyroFork-2.2.0/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/set_chat_photo.py` & `PyroFork-2.2.0/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/set_chat_protected_content.py` & `PyroFork-2.2.0/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/set_chat_title.py` & `PyroFork-2.2.0/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/set_chat_username.py` & `PyroFork-2.2.0/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/set_send_as_chat.py` & `PyroFork-2.2.0/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/set_slow_mode.py` & `PyroFork-2.2.0/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/unarchive_chats.py` & `PyroFork-2.2.0/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/unban_chat_member.py` & `PyroFork-2.2.0/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/unhide_general_topic.py` & `PyroFork-2.2.0/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/unpin_all_chat_messages.py` & `PyroFork-2.2.0/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/chats/unpin_chat_message.py` & `PyroFork-2.2.0/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/contacts/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/contacts/add_contact.py` & `PyroFork-2.2.0/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/contacts/delete_contacts.py` & `PyroFork-2.2.0/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/contacts/get_contacts.py` & `PyroFork-2.2.0/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/contacts/get_contacts_count.py` & `PyroFork-2.2.0/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/contacts/import_contacts.py` & `PyroFork-2.2.0/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_callback_query.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_chat_join_request.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_chat_member_updated.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_chosen_inline_result.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_deleted_messages.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_disconnect.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_edited_message.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_inline_query.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_message.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_poll.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_raw_update.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/decorators/on_user_status.py` & `PyroFork-2.2.0/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/approve_chat_join_request.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/create_chat_invite_link.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/decline_chat_join_request.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/export_chat_invite_link.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_invite_link.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/get_chat_join_requests.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `PyroFork-2.2.0/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/copy_media_group.py` & `PyroFork-2.2.0/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/copy_message.py` & `PyroFork-2.2.0/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/delete_messages.py` & `PyroFork-2.2.0/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/download_media.py` & `PyroFork-2.2.0/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/edit_inline_caption.py` & `PyroFork-2.2.0/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/edit_inline_media.py` & `PyroFork-2.2.0/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/edit_inline_reply_markup.py` & `PyroFork-2.2.0/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/edit_inline_text.py` & `PyroFork-2.2.0/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/edit_message_caption.py` & `PyroFork-2.2.0/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/edit_message_media.py` & `PyroFork-2.2.0/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/edit_message_reply_markup.py` & `PyroFork-2.2.0/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/edit_message_text.py` & `PyroFork-2.2.0/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/forward_messages.py` & `PyroFork-2.2.0/pyrogram/methods/messages/forward_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         from_chat_id: Union[int, str],
         message_ids: Union[int, Iterable[int]],
         message_thread_id: int = None,
         disable_notification: bool = None,
         schedule_date: datetime = None,
-        protect_content: bool = None
+        protect_content: bool = None,
+        drop_author: bool = None
     ) -> Union["types.Message", List["types.Message"]]:
         """Forward messages of any kind.
 
         .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
@@ -63,14 +64,17 @@
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             protect_content (``bool``, *optional*):
                 Protects the contents of the sent message from forwarding and saving.
 
+            drop_author (``bool``, *optional*):
+                Forwards messages without quoting the original author
+
         Returns:
             :obj:`~pyrogram.types.Message` | List of :obj:`~pyrogram.types.Message`: In case *message_ids* was not
             a list, a single message is returned, otherwise a list of messages is returned.
 
         Example:
             .. code-block:: python
 
@@ -89,15 +93,16 @@
                 to_peer=await self.resolve_peer(chat_id),
                 from_peer=await self.resolve_peer(from_chat_id),
                 id=message_ids,
                 top_msg_id=message_thread_id,
                 silent=disable_notification or None,
                 random_id=[self.rnd_id() for _ in message_ids],
                 schedule_date=utils.datetime_to_timestamp(schedule_date),
-                noforwards=protect_content
+                noforwards=protect_content,
+                drop_author=drop_author
             )
         )
 
         forwarded_messages = []
 
         users = {i.id: i for i in r.users}
         chats = {i.id: i for i in r.chats}
```

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/get_chat_history.py` & `PyroFork-2.2.0/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/get_chat_history_count.py` & `PyroFork-2.2.0/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `PyroFork-2.2.0/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/get_discussion_message.py` & `PyroFork-2.2.0/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/get_discussion_replies.py` & `PyroFork-2.2.0/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/get_discussion_replies_count.py` & `PyroFork-2.2.0/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/get_media_group.py` & `PyroFork-2.2.0/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/get_messages.py` & `PyroFork-2.2.0/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/inline_session.py` & `PyroFork-2.2.0/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/read_chat_history.py` & `PyroFork-2.2.0/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/retract_vote.py` & `PyroFork-2.2.0/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/search_global.py` & `PyroFork-2.2.0/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/search_global_count.py` & `PyroFork-2.2.0/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/search_messages.py` & `PyroFork-2.2.0/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/search_messages_count.py` & `PyroFork-2.2.0/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_animation.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_audio.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_cached_media.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_chat_action.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_contact.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_dice.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_document.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_location.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_media_group.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_message.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_photo.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_poll.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_reaction.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_sticker.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_venue.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_video.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_video_note.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/send_voice.py` & `PyroFork-2.2.0/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/stop_poll.py` & `PyroFork-2.2.0/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/stream_media.py` & `PyroFork-2.2.0/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/messages/vote_poll.py` & `PyroFork-2.2.0/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/password/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/password/change_cloud_password.py` & `PyroFork-2.2.0/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/password/enable_cloud_password.py` & `PyroFork-2.2.0/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/password/remove_cloud_password.py` & `PyroFork-2.2.0/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/stickers/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/stickers/add_sticker_to_set.py` & `PyroFork-2.2.0/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/stickers/create_sticker_set.py` & `PyroFork-2.2.0/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/stickers/get_sticker_set.py` & `PyroFork-2.2.0/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/block_user.py` & `PyroFork-2.2.0/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/delete_profile_photos.py` & `PyroFork-2.2.0/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/get_chat_photos.py` & `PyroFork-2.2.0/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/get_chat_photos_count.py` & `PyroFork-2.2.0/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/get_common_chats.py` & `PyroFork-2.2.0/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/get_default_emoji_statuses.py` & `PyroFork-2.2.0/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/get_me.py` & `PyroFork-2.2.0/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/get_users.py` & `PyroFork-2.2.0/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/set_emoji_status.py` & `PyroFork-2.2.0/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/set_profile_photo.py` & `PyroFork-2.2.0/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/set_username.py` & `PyroFork-2.2.0/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/unblock_user.py` & `PyroFork-2.2.0/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/users/update_profile.py` & `PyroFork-2.2.0/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/__init__.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/add_handler.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/compose.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/export_session_string.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/idle.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/remove_handler.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/restart.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/run.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/start.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/stop.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/methods/utilities/stop_transmission.py` & `PyroFork-2.2.0/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/mime_types.py` & `PyroFork-2.2.0/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/parser/__init__.py` & `PyroFork-2.2.0/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/parser/html.py` & `PyroFork-2.2.0/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/parser/markdown.py` & `PyroFork-2.2.0/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/parser/parser.py` & `PyroFork-2.2.0/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/parser/utils.py` & `PyroFork-2.2.0/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/__init__.py` & `PyroFork-2.2.0/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/__init__.py` & `PyroFork-2.2.0/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/future_salt.py` & `PyroFork-2.2.0/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/future_salts.py` & `PyroFork-2.2.0/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/gzip_packed.py` & `PyroFork-2.2.0/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/list.py` & `PyroFork-2.2.0/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/message.py` & `PyroFork-2.2.0/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/msg_container.py` & `PyroFork-2.2.0/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/primitives/__init__.py` & `PyroFork-2.2.0/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/primitives/bool.py` & `PyroFork-2.2.0/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/primitives/bytes.py` & `PyroFork-2.2.0/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/primitives/double.py` & `PyroFork-2.2.0/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/primitives/int.py` & `PyroFork-2.2.0/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/primitives/string.py` & `PyroFork-2.2.0/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/primitives/vector.py` & `PyroFork-2.2.0/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/raw/core/tl_object.py` & `PyroFork-2.2.0/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/session/__init__.py` & `PyroFork-2.2.0/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/session/auth.py` & `PyroFork-2.2.0/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/session/internals/__init__.py` & `PyroFork-2.2.0/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/session/internals/data_center.py` & `PyroFork-2.2.0/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/session/internals/msg_factory.py` & `PyroFork-2.2.0/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/session/internals/msg_id.py` & `PyroFork-2.2.0/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/session/internals/seq_no.py` & `PyroFork-2.2.0/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/session/session.py` & `PyroFork-2.2.0/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/storage/__init__.py` & `PyroFork-2.2.0/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/storage/file_storage.py` & `PyroFork-2.2.0/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/storage/memory_storage.py` & `PyroFork-2.2.0/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/storage/mongo_storage.py` & `PyroFork-2.2.0/pyrogram/storage/mongo_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 import asyncio
 import inspect
 import time
 from typing import List, Tuple, Any
 
-from motor.motor_asyncio import AsyncIOMotorClient
+from async_pymongo import AsyncClient
 from pymongo import UpdateOne
 from pyrogram.storage.storage import Storage
 from pyrogram.storage.sqlite_storage import get_input_peer
 
 
 class MongoStorage(Storage):
     """
-    config (``dict``)
-        Mongodb config as dict, e.g.: *dict(uri="mongodb://...", db_name="pyrofork-session", remove_peers=False)*.
-        Only applicable for new sessions.
+    Initializes a new session.
+
+    Parameters:
+        - name (`str`):
+            The session name used for database name.
+
+        - uri (`str`):
+            MongoDB Connection String URI.
+            For more information refer to https://www.mongodb.com/docs/manual/reference/connection-string
+
+        - remove_peers (`bool`, *optional*):
+            Flag to remove data in the peers collection. If set to True, 
+            the data related to peers will be removed everytime client log out. 
+            If set to False or None, the data will not be removed.
+
+    Example:
+        session = MongoStorage("my_session", uri="mongodb://...", remove_peers=True)
     """
     lock: asyncio.Lock
     USERNAME_TTL = 8 * 60 * 60
 
-    def __init__(self, config: dict):
-        super().__init__('')
-        db_name = "pyrofork-session"
-        db_uri = config["uri"]
-        remove_peers = False
-        if "db_name" in config:
-            db_name = config["db_name"]
-        if "remove_peers" in config:
-            remove_peers = config["remove_peers"]
-        database = AsyncIOMotorClient(db_uri)[db_name]
+    def __init__(self, name: str, uri: str, remove_peers: bool = False):
+        super().__init__(name=name)
+        database = AsyncClient(uri)[name]
         self.lock = asyncio.Lock()
         self.database = database
         self._peer = database['peers']
         self._session = database['session']
         self._remove_peers = remove_peers
 
     async def open(self):
```

### Comparing `PyroFork-2.1.8/pyrogram/storage/sqlite_storage.py` & `PyroFork-2.2.0/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/storage/storage.py` & `PyroFork-2.2.0/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/sync.py` & `PyroFork-2.2.0/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/__init__.py` & `PyroFork-2.2.0/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/authorization/__init__.py` & `PyroFork-2.2.0/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/authorization/sent_code.py` & `PyroFork-2.2.0/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/authorization/terms_of_service.py` & `PyroFork-2.2.0/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/__init__.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/callback_game.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/callback_query.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/force_reply.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/game_high_score.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/login_url.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/menu_button.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/bots_and_keyboards/web_app_info.py` & `PyroFork-2.2.0/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/__init__.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/chosen_inline_result.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_animation.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_article.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_audio.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_contact.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_document.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_location.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_photo.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_venue.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_video.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/inline_mode/inline_query_result_voice.py` & `PyroFork-2.2.0/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_media/__init__.py` & `PyroFork-2.2.0/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_media/input_media.py` & `PyroFork-2.2.0/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_media/input_media_animation.py` & `PyroFork-2.2.0/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_media/input_media_audio.py` & `PyroFork-2.2.0/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_media/input_media_document.py` & `PyroFork-2.2.0/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_media/input_media_photo.py` & `PyroFork-2.2.0/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_media/input_media_video.py` & `PyroFork-2.2.0/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_media/input_phone_contact.py` & `PyroFork-2.2.0/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_message_content/__init__.py` & `PyroFork-2.2.0/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_message_content/input_message_content.py` & `PyroFork-2.2.0/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/input_message_content/input_text_message_content.py` & `PyroFork-2.2.0/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/list.py` & `PyroFork-2.2.0/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/__init__.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/animation.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/audio.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/contact.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/dice.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/document.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/game.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/location.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/message.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -8041,1534 +8041,1560 @@
 0001f680: 2020 2020 2020 206d 6573 7361 6765 5f74         message_t
 0001f690: 6872 6561 645f 6964 3a20 696e 7420 3d20  hread_id: int = 
 0001f6a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6469  None,.        di
 0001f6b0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
 0001f6c0: 6f6e 3a20 626f 6f6c 203d 204e 6f6e 652c  on: bool = None,
 0001f6d0: 0a20 2020 2020 2020 2073 6368 6564 756c  .        schedul
 0001f6e0: 655f 6461 7465 3a20 6461 7465 7469 6d65  e_date: datetime
-0001f6f0: 203d 204e 6f6e 650a 2020 2020 2920 2d3e   = None.    ) ->
-0001f700: 2055 6e69 6f6e 5b22 7479 7065 732e 4d65   Union["types.Me
-0001f710: 7373 6167 6522 2c20 4c69 7374 5b22 7479  ssage", List["ty
-0001f720: 7065 732e 4d65 7373 6167 6522 5d5d 3a0a  pes.Message"]]:.
-0001f730: 2020 2020 2020 2020 2222 2242 6f75 6e64          """Bound
-0001f740: 206d 6574 686f 6420 2a66 6f72 7761 7264   method *forward
-0001f750: 2a20 6f66 203a 6f62 6a3a 607e 7079 726f  * of :obj:`~pyro
-0001f760: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
-0001f770: 6765 602e 0a0a 2020 2020 2020 2020 5573  ge`...        Us
-0001f780: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
-0001f790: 666f 723a 0a0a 2020 2020 2020 2020 2e2e  for:..        ..
-0001f7a0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-0001f7b0: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-0001f7c0: 2020 6177 6169 7420 636c 6965 6e74 2e66    await client.f
-0001f7d0: 6f72 7761 7264 5f6d 6573 7361 6765 7328  orward_messages(
-0001f7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f7f0: 2063 6861 745f 6964 3d63 6861 745f 6964   chat_id=chat_id
-0001f800: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001f810: 2020 6672 6f6d 5f63 6861 745f 6964 3d6d    from_chat_id=m
-0001f820: 6573 7361 6765 2e63 6861 742e 6964 2c0a  essage.chat.id,.
-0001f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f840: 6d65 7373 6167 655f 6964 733d 6d65 7373  message_ids=mess
-0001f850: 6167 652e 6964 0a20 2020 2020 2020 2020  age.id.         
-0001f860: 2020 2029 0a0a 2020 2020 2020 2020 4578     )..        Ex
-0001f870: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
-0001f880: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
-0001f890: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
-0001f8a0: 2020 2020 2020 2020 2020 2061 7761 6974             await
-0001f8b0: 206d 6573 7361 6765 2e66 6f72 7761 7264   message.forward
-0001f8c0: 2863 6861 745f 6964 290a 0a20 2020 2020  (chat_id)..     
-0001f8d0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
-0001f8e0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-0001f8f0: 6964 2028 6060 696e 7460 6020 7c20 6060  id (``int`` | ``
-0001f900: 7374 7260 6029 3a0a 2020 2020 2020 2020  str``):.        
-0001f910: 2020 2020 2020 2020 556e 6971 7565 2069          Unique i
-0001f920: 6465 6e74 6966 6965 7220 2869 6e74 2920  dentifier (int) 
-0001f930: 6f72 2075 7365 726e 616d 6520 2873 7472  or username (str
-0001f940: 2920 6f66 2074 6865 2074 6172 6765 7420  ) of the target 
-0001f950: 6368 6174 2e0a 2020 2020 2020 2020 2020  chat..          
-0001f960: 2020 2020 2020 466f 7220 796f 7572 2070        For your p
-0001f970: 6572 736f 6e61 6c20 636c 6f75 6420 2853  ersonal cloud (S
-0001f980: 6176 6564 204d 6573 7361 6765 7329 2079  aved Messages) y
-0001f990: 6f75 2063 616e 2073 696d 706c 7920 7573  ou can simply us
-0001f9a0: 6520 226d 6522 206f 7220 2273 656c 6622  e "me" or "self"
-0001f9b0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001f9c0: 2020 466f 7220 6120 636f 6e74 6163 7420    For a contact 
-0001f9d0: 7468 6174 2065 7869 7374 7320 696e 2079  that exists in y
-0001f9e0: 6f75 7220 5465 6c65 6772 616d 2061 6464  our Telegram add
-0001f9f0: 7265 7373 2062 6f6f 6b20 796f 7520 6361  ress book you ca
-0001fa00: 6e20 7573 6520 6869 7320 7068 6f6e 6520  n use his phone 
-0001fa10: 6e75 6d62 6572 2028 7374 7229 2e0a 0a20  number (str)... 
-0001fa20: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-0001fa30: 6765 5f74 6872 6561 645f 6964 2028 6060  ge_thread_id (``
-0001fa40: 696e 7460 602c 202a 6f70 7469 6f6e 616c  int``, *optional
-0001fa50: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-0001fa60: 2020 2020 556e 6971 7565 2069 6465 6e74      Unique ident
-0001fa70: 6966 6965 7220 6f66 2061 206d 6573 7361  ifier of a messa
-0001fa80: 6765 2074 6872 6561 6420 746f 2077 6869  ge thread to whi
-0001fa90: 6368 2074 6865 206d 6573 7361 6765 2062  ch the message b
-0001faa0: 656c 6f6e 6773 3b20 666f 7220 7375 7065  elongs; for supe
-0001fab0: 7267 726f 7570 7320 6f6e 6c79 0a0a 2020  rgroups only..  
-0001fac0: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
-0001fad0: 655f 6e6f 7469 6669 6361 7469 6f6e 2028  e_notification (
-0001fae0: 6060 626f 6f6c 6060 2c20 2a6f 7074 696f  ``bool``, *optio
-0001faf0: 6e61 6c2a 293a 0a20 2020 2020 2020 2020  nal*):.         
-0001fb00: 2020 2020 2020 2053 656e 6473 2074 6865         Sends the
-0001fb10: 206d 6573 7361 6765 2073 696c 656e 746c   message silentl
-0001fb20: 792e 0a20 2020 2020 2020 2020 2020 2020  y..             
-0001fb30: 2020 2055 7365 7273 2077 696c 6c20 7265     Users will re
-0001fb40: 6365 6976 6520 6120 6e6f 7469 6669 6361  ceive a notifica
-0001fb50: 7469 6f6e 2077 6974 6820 6e6f 2073 6f75  tion with no sou
-0001fb60: 6e64 2e0a 0a20 2020 2020 2020 2020 2020  nd...           
-0001fb70: 2073 6368 6564 756c 655f 6461 7465 2028   schedule_date (
-0001fb80: 3a70 793a 6f62 6a3a 607e 6461 7465 7469  :py:obj:`~dateti
-0001fb90: 6d65 2e64 6174 6574 696d 6560 2c20 2a6f  me.datetime`, *o
-0001fba0: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-0001fbb0: 2020 2020 2020 2020 2020 2044 6174 6520             Date 
-0001fbc0: 7768 656e 2074 6865 206d 6573 7361 6765  when the message
-0001fbd0: 2077 696c 6c20 6265 2061 7574 6f6d 6174   will be automat
-0001fbe0: 6963 616c 6c79 2073 656e 742e 0a0a 2020  ically sent...  
-0001fbf0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0001fc00: 2020 2020 2020 2020 2020 204f 6e20 7375             On su
-0001fc10: 6363 6573 732c 2074 6865 2066 6f72 7761  ccess, the forwa
-0001fc20: 7264 6564 204d 6573 7361 6765 2069 7320  rded Message is 
-0001fc30: 7265 7475 726e 6564 2e0a 0a20 2020 2020  returned...     
-0001fc40: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-0001fc50: 2020 2020 2020 2052 5043 4572 726f 723a         RPCError:
-0001fc60: 2049 6e20 6361 7365 206f 6620 6120 5465   In case of a Te
-0001fc70: 6c65 6772 616d 2052 5043 2065 7272 6f72  legram RPC error
-0001fc80: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0001fc90: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0001fca0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-0001fcb0: 666f 7277 6172 645f 6d65 7373 6167 6573  forward_messages
-0001fcc0: 280a 2020 2020 2020 2020 2020 2020 6368  (.            ch
-0001fcd0: 6174 5f69 643d 6368 6174 5f69 642c 0a20  at_id=chat_id,. 
-0001fce0: 2020 2020 2020 2020 2020 2066 726f 6d5f             from_
-0001fcf0: 6368 6174 5f69 643d 7365 6c66 2e63 6861  chat_id=self.cha
-0001fd00: 742e 6964 2c0a 2020 2020 2020 2020 2020  t.id,.          
-0001fd10: 2020 6d65 7373 6167 655f 6964 733d 7365    message_ids=se
-0001fd20: 6c66 2e69 642c 0a20 2020 2020 2020 2020  lf.id,.         
-0001fd30: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
-0001fd40: 645f 6964 3d6d 6573 7361 6765 5f74 6872  d_id=message_thr
-0001fd50: 6561 645f 6964 2c0a 2020 2020 2020 2020  ead_id,.        
-0001fd60: 2020 2020 6469 7361 626c 655f 6e6f 7469      disable_noti
-0001fd70: 6669 6361 7469 6f6e 3d64 6973 6162 6c65  fication=disable
-0001fd80: 5f6e 6f74 6966 6963 6174 696f 6e2c 0a20  _notification,. 
-0001fd90: 2020 2020 2020 2020 2020 2073 6368 6564             sched
-0001fda0: 756c 655f 6461 7465 3d73 6368 6564 756c  ule_date=schedul
-0001fdb0: 655f 6461 7465 0a20 2020 2020 2020 2029  e_date.        )
-0001fdc0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-0001fdd0: 636f 7079 280a 2020 2020 2020 2020 7365  copy(.        se
-0001fde0: 6c66 2c0a 2020 2020 2020 2020 6368 6174  lf,.        chat
-0001fdf0: 5f69 643a 2055 6e69 6f6e 5b69 6e74 2c20  _id: Union[int, 
-0001fe00: 7374 725d 2c0a 2020 2020 2020 2020 6361  str],.        ca
-0001fe10: 7074 696f 6e3a 2073 7472 203d 204e 6f6e  ption: str = Non
-0001fe20: 652c 0a20 2020 2020 2020 2070 6172 7365  e,.        parse
-0001fe30: 5f6d 6f64 653a 204f 7074 696f 6e61 6c5b  _mode: Optional[
-0001fe40: 2265 6e75 6d73 2e50 6172 7365 4d6f 6465  "enums.ParseMode
-0001fe50: 225d 203d 204e 6f6e 652c 0a20 2020 2020  "] = None,.     
-0001fe60: 2020 2063 6170 7469 6f6e 5f65 6e74 6974     caption_entit
-0001fe70: 6965 733a 204c 6973 745b 2274 7970 6573  ies: List["types
-0001fe80: 2e4d 6573 7361 6765 456e 7469 7479 225d  .MessageEntity"]
-0001fe90: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0001fea0: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-0001feb0: 6174 696f 6e3a 2062 6f6f 6c20 3d20 4e6f  ation: bool = No
-0001fec0: 6e65 2c0a 2020 2020 2020 2020 6d65 7373  ne,.        mess
-0001fed0: 6167 655f 7468 7265 6164 5f69 643a 2069  age_thread_id: i
-0001fee0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-0001fef0: 2020 2072 6570 6c79 5f74 6f5f 6d65 7373     reply_to_mess
-0001ff00: 6167 655f 6964 3a20 696e 7420 3d20 4e6f  age_id: int = No
-0001ff10: 6e65 2c0a 2020 2020 2020 2020 7363 6865  ne,.        sche
-0001ff20: 6475 6c65 5f64 6174 653a 2064 6174 6574  dule_date: datet
-0001ff30: 696d 6520 3d20 4e6f 6e65 2c0a 2020 2020  ime = None,.    
-0001ff40: 2020 2020 7072 6f74 6563 745f 636f 6e74      protect_cont
-0001ff50: 656e 743a 2062 6f6f 6c20 3d20 4e6f 6e65  ent: bool = None
-0001ff60: 2c0a 2020 2020 2020 2020 7265 706c 795f  ,.        reply_
-0001ff70: 6d61 726b 7570 3a20 556e 696f 6e5b 0a20  markup: Union[. 
-0001ff80: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-0001ff90: 732e 496e 6c69 6e65 4b65 7962 6f61 7264  s.InlineKeyboard
-0001ffa0: 4d61 726b 7570 222c 0a20 2020 2020 2020  Markup",.       
-0001ffb0: 2020 2020 2022 7479 7065 732e 5265 706c       "types.Repl
-0001ffc0: 794b 6579 626f 6172 644d 6172 6b75 7022  yKeyboardMarkup"
-0001ffd0: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
-0001ffe0: 7970 6573 2e52 6570 6c79 4b65 7962 6f61  ypes.ReplyKeyboa
-0001fff0: 7264 5265 6d6f 7665 222c 0a20 2020 2020  rdRemove",.     
-00020000: 2020 2020 2020 2022 7479 7065 732e 466f         "types.Fo
-00020010: 7263 6552 6570 6c79 220a 2020 2020 2020  rceReply".      
-00020020: 2020 5d20 3d20 6f62 6a65 6374 0a20 2020    ] = object.   
-00020030: 2029 202d 3e20 556e 696f 6e5b 2274 7970   ) -> Union["typ
-00020040: 6573 2e4d 6573 7361 6765 222c 204c 6973  es.Message", Lis
-00020050: 745b 2274 7970 6573 2e4d 6573 7361 6765  t["types.Message
-00020060: 225d 5d3a 0a20 2020 2020 2020 2022 2222  "]]:.        """
-00020070: 426f 756e 6420 6d65 7468 6f64 202a 636f  Bound method *co
-00020080: 7079 2a20 6f66 203a 6f62 6a3a 607e 7079  py* of :obj:`~py
-00020090: 726f 6772 616d 2e74 7970 6573 2e4d 6573  rogram.types.Mes
-000200a0: 7361 6765 602e 0a0a 2020 2020 2020 2020  sage`...        
-000200b0: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
-000200c0: 7420 666f 723a 0a0a 2020 2020 2020 2020  t for:..        
-000200d0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-000200e0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-000200f0: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
-00020100: 2e63 6f70 795f 6d65 7373 6167 6528 0a20  .copy_message(. 
-00020110: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00020120: 6861 745f 6964 3d63 6861 745f 6964 2c0a  hat_id=chat_id,.
-00020130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020140: 6672 6f6d 5f63 6861 745f 6964 3d6d 6573  from_chat_id=mes
-00020150: 7361 6765 2e63 6861 742e 6964 2c0a 2020  sage.chat.id,.  
-00020160: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00020170: 7373 6167 655f 6964 3d6d 6573 7361 6765  ssage_id=message
-00020180: 2e69 640a 2020 2020 2020 2020 2020 2020  .id.            
-00020190: 290a 0a20 2020 2020 2020 2045 7861 6d70  )..        Examp
-000201a0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-000201b0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-000201c0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-000201d0: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
-000201e0: 7373 6167 652e 636f 7079 2863 6861 745f  ssage.copy(chat_
-000201f0: 6964 290a 0a20 2020 2020 2020 2050 6172  id)..        Par
-00020200: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
-00020210: 2020 2020 2063 6861 745f 6964 2028 6060       chat_id (``
-00020220: 696e 7460 6020 7c20 6060 7374 7260 6029  int`` | ``str``)
-00020230: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00020240: 2020 556e 6971 7565 2069 6465 6e74 6966    Unique identif
-00020250: 6965 7220 2869 6e74 2920 6f72 2075 7365  ier (int) or use
-00020260: 726e 616d 6520 2873 7472 2920 6f66 2074  rname (str) of t
-00020270: 6865 2074 6172 6765 7420 6368 6174 2e0a  he target chat..
-00020280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020290: 466f 7220 796f 7572 2070 6572 736f 6e61  For your persona
-000202a0: 6c20 636c 6f75 6420 2853 6176 6564 204d  l cloud (Saved M
-000202b0: 6573 7361 6765 7329 2079 6f75 2063 616e  essages) you can
-000202c0: 2073 696d 706c 7920 7573 6520 226d 6522   simply use "me"
-000202d0: 206f 7220 2273 656c 6622 2e0a 2020 2020   or "self"..    
-000202e0: 2020 2020 2020 2020 2020 2020 466f 7220              For 
-000202f0: 6120 636f 6e74 6163 7420 7468 6174 2065  a contact that e
-00020300: 7869 7374 7320 696e 2079 6f75 7220 5465  xists in your Te
-00020310: 6c65 6772 616d 2061 6464 7265 7373 2062  legram address b
-00020320: 6f6f 6b20 796f 7520 6361 6e20 7573 6520  ook you can use 
-00020330: 6869 7320 7068 6f6e 6520 6e75 6d62 6572  his phone number
-00020340: 2028 7374 7229 2e0a 0a20 2020 2020 2020   (str)...       
-00020350: 2020 2020 2063 6170 7469 6f6e 2028 6060       caption (``
-00020360: 7374 7269 6e67 6060 2c20 2a6f 7074 696f  string``, *optio
-00020370: 6e61 6c2a 293a 0a20 2020 2020 2020 2020  nal*):.         
-00020380: 2020 2020 2020 204e 6577 2063 6170 7469         New capti
-00020390: 6f6e 2066 6f72 206d 6564 6961 2c20 302d  on for media, 0-
-000203a0: 3130 3234 2063 6861 7261 6374 6572 7320  1024 characters 
-000203b0: 6166 7465 7220 656e 7469 7469 6573 2070  after entities p
-000203c0: 6172 7369 6e67 2e0a 2020 2020 2020 2020  arsing..        
-000203d0: 2020 2020 2020 2020 4966 206e 6f74 2073          If not s
-000203e0: 7065 6369 6669 6564 2c20 7468 6520 6f72  pecified, the or
-000203f0: 6967 696e 616c 2063 6170 7469 6f6e 2069  iginal caption i
-00020400: 7320 6b65 7074 2e0a 2020 2020 2020 2020  s kept..        
-00020410: 2020 2020 2020 2020 5061 7373 2022 2220          Pass "" 
-00020420: 2865 6d70 7479 2073 7472 696e 6729 2074  (empty string) t
-00020430: 6f20 7265 6d6f 7665 2074 6865 2063 6170  o remove the cap
-00020440: 7469 6f6e 2e0a 0a20 2020 2020 2020 2020  tion...         
-00020450: 2020 2070 6172 7365 5f6d 6f64 6520 283a     parse_mode (:
-00020460: 6f62 6a3a 607e 7079 726f 6772 616d 2e65  obj:`~pyrogram.e
-00020470: 6e75 6d73 2e50 6172 7365 4d6f 6465 602c  nums.ParseMode`,
-00020480: 202a 6f70 7469 6f6e 616c 2a29 3a0a 2020   *optional*):.  
-00020490: 2020 2020 2020 2020 2020 2020 2020 4279                By
-000204a0: 2064 6566 6175 6c74 2c20 7465 7874 7320   default, texts 
-000204b0: 6172 6520 7061 7273 6564 2075 7369 6e67  are parsed using
-000204c0: 2062 6f74 6820 4d61 726b 646f 776e 2061   both Markdown a
-000204d0: 6e64 2048 544d 4c20 7374 796c 6573 2e0a  nd HTML styles..
-000204e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000204f0: 596f 7520 6361 6e20 636f 6d62 696e 6520  You can combine 
-00020500: 626f 7468 2073 796e 7461 7865 7320 746f  both syntaxes to
-00020510: 6765 7468 6572 2e0a 0a20 2020 2020 2020  gether...       
-00020520: 2020 2020 2063 6170 7469 6f6e 5f65 6e74       caption_ent
-00020530: 6974 6965 7320 284c 6973 7420 6f66 203a  ities (List of :
-00020540: 6f62 6a3a 607e 7079 726f 6772 616d 2e74  obj:`~pyrogram.t
-00020550: 7970 6573 2e4d 6573 7361 6765 456e 7469  ypes.MessageEnti
-00020560: 7479 6029 3a0a 2020 2020 2020 2020 2020  ty`):.          
-00020570: 2020 2020 2020 4c69 7374 206f 6620 7370        List of sp
-00020580: 6563 6961 6c20 656e 7469 7469 6573 2074  ecial entities t
-00020590: 6861 7420 6170 7065 6172 2069 6e20 7468  hat appear in th
-000205a0: 6520 6e65 7720 6361 7074 696f 6e2c 2077  e new caption, w
-000205b0: 6869 6368 2063 616e 2062 6520 7370 6563  hich can be spec
-000205c0: 6966 6965 6420 696e 7374 6561 6420 6f66  ified instead of
-000205d0: 202a 7061 7273 655f 6d6f 6465 2a2e 0a0a   *parse_mode*...
-000205e0: 2020 2020 2020 2020 2020 2020 6469 7361              disa
-000205f0: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00020600: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
-00020610: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
-00020620: 2020 2020 2020 2020 2053 656e 6473 2074           Sends t
-00020630: 6865 206d 6573 7361 6765 2073 696c 656e  he message silen
-00020640: 746c 792e 0a20 2020 2020 2020 2020 2020  tly..           
-00020650: 2020 2020 2055 7365 7273 2077 696c 6c20       Users will 
-00020660: 7265 6365 6976 6520 6120 6e6f 7469 6669  receive a notifi
-00020670: 6361 7469 6f6e 2077 6974 6820 6e6f 2073  cation with no s
-00020680: 6f75 6e64 2e0a 0a20 2020 2020 2020 2020  ound...         
-00020690: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
-000206a0: 645f 6964 2028 6060 696e 7460 602c 202a  d_id (``int``, *
-000206b0: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
-000206c0: 2020 2020 2020 2020 2020 2020 556e 6971              Uniq
-000206d0: 7565 2069 6465 6e74 6966 6965 7220 666f  ue identifier fo
-000206e0: 7220 7468 6520 7461 7267 6574 206d 6573  r the target mes
-000206f0: 7361 6765 2074 6872 6561 6420 2874 6f70  sage thread (top
-00020700: 6963 2920 6f66 2074 6865 2066 6f72 756d  ic) of the forum
-00020710: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020720: 2020 666f 7220 666f 7275 6d20 7375 7065    for forum supe
-00020730: 7267 726f 7570 7320 6f6e 6c79 2e0a 0a20  rgroups only... 
-00020740: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
-00020750: 5f74 6f5f 6d65 7373 6167 655f 6964 2028  _to_message_id (
-00020760: 6060 696e 7460 602c 202a 6f70 7469 6f6e  ``int``, *option
-00020770: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
-00020780: 2020 2020 2020 4966 2074 6865 206d 6573        If the mes
-00020790: 7361 6765 2069 7320 6120 7265 706c 792c  sage is a reply,
-000207a0: 2049 4420 6f66 2074 6865 206f 7269 6769   ID of the origi
-000207b0: 6e61 6c20 6d65 7373 6167 652e 0a0a 2020  nal message...  
-000207c0: 2020 2020 2020 2020 2020 7363 6865 6475            schedu
-000207d0: 6c65 5f64 6174 6520 283a 7079 3a6f 626a  le_date (:py:obj
-000207e0: 3a60 7e64 6174 6574 696d 652e 6461 7465  :`~datetime.date
-000207f0: 7469 6d65 602c 202a 6f70 7469 6f6e 616c  time`, *optional
-00020800: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-00020810: 2020 2020 4461 7465 2077 6865 6e20 7468      Date when th
-00020820: 6520 6d65 7373 6167 6520 7769 6c6c 2062  e message will b
-00020830: 6520 6175 746f 6d61 7469 6361 6c6c 7920  e automatically 
-00020840: 7365 6e74 2e0a 0a20 2020 2020 2020 2020  sent...         
-00020850: 2020 2070 726f 7465 6374 5f63 6f6e 7465     protect_conte
-00020860: 6e74 2028 6060 626f 6f6c 6060 2c20 2a6f  nt (``bool``, *o
-00020870: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-00020880: 2020 2020 2020 2020 2020 2050 726f 7465             Prote
-00020890: 6374 7320 7468 6520 636f 6e74 656e 7473  cts the contents
-000208a0: 206f 6620 7468 6520 7365 6e74 206d 6573   of the sent mes
-000208b0: 7361 6765 2066 726f 6d20 666f 7277 6172  sage from forwar
-000208c0: 6469 6e67 2061 6e64 2073 6176 696e 672e  ding and saving.
-000208d0: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000208e0: 706c 795f 6d61 726b 7570 2028 3a6f 626a  ply_markup (:obj
-000208f0: 3a60 7e70 7972 6f67 7261 6d2e 7479 7065  :`~pyrogram.type
-00020900: 732e 496e 6c69 6e65 4b65 7962 6f61 7264  s.InlineKeyboard
-00020910: 4d61 726b 7570 6020 7c20 3a6f 626a 3a60  Markup` | :obj:`
-00020920: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
-00020930: 5265 706c 794b 6579 626f 6172 644d 6172  ReplyKeyboardMar
-00020940: 6b75 7060 207c 203a 6f62 6a3a 607e 7079  kup` | :obj:`~py
-00020950: 726f 6772 616d 2e74 7970 6573 2e52 6570  rogram.types.Rep
-00020960: 6c79 4b65 7962 6f61 7264 5265 6d6f 7665  lyKeyboardRemove
-00020970: 6020 7c20 3a6f 626a 3a60 7e70 7972 6f67  ` | :obj:`~pyrog
-00020980: 7261 6d2e 7479 7065 732e 466f 7263 6552  ram.types.ForceR
-00020990: 6570 6c79 602c 202a 6f70 7469 6f6e 616c  eply`, *optional
-000209a0: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-000209b0: 2020 2020 4164 6469 7469 6f6e 616c 2069      Additional i
-000209c0: 6e74 6572 6661 6365 206f 7074 696f 6e73  nterface options
-000209d0: 2e20 416e 206f 626a 6563 7420 666f 7220  . An object for 
-000209e0: 616e 2069 6e6c 696e 6520 6b65 7962 6f61  an inline keyboa
-000209f0: 7264 2c20 6375 7374 6f6d 2072 6570 6c79  rd, custom reply
-00020a00: 206b 6579 626f 6172 642c 0a20 2020 2020   keyboard,.     
-00020a10: 2020 2020 2020 2020 2020 2069 6e73 7472             instr
-00020a20: 7563 7469 6f6e 7320 746f 2072 656d 6f76  uctions to remov
-00020a30: 6520 7265 706c 7920 6b65 7962 6f61 7264  e reply keyboard
-00020a40: 206f 7220 746f 2066 6f72 6365 2061 2072   or to force a r
-00020a50: 6570 6c79 2066 726f 6d20 7468 6520 7573  eply from the us
-00020a60: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
-00020a70: 2020 2020 4966 206e 6f74 2073 7065 6369      If not speci
-00020a80: 6669 6564 2c20 7468 6520 6f72 6967 696e  fied, the origin
-00020a90: 616c 2072 6570 6c79 206d 6172 6b75 7020  al reply markup 
-00020aa0: 6973 206b 6570 742e 0a20 2020 2020 2020  is kept..       
-00020ab0: 2020 2020 2020 2020 2050 6173 7320 4e6f           Pass No
-00020ac0: 6e65 2074 6f20 7265 6d6f 7665 2074 6865  ne to remove the
-00020ad0: 2072 6570 6c79 206d 6172 6b75 702e 0a0a   reply markup...
-00020ae0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00020af0: 0a20 2020 2020 2020 2020 2020 203a 6f62  .            :ob
-00020b00: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
-00020b10: 6573 2e4d 6573 7361 6765 603a 204f 6e20  es.Message`: On 
-00020b20: 7375 6363 6573 732c 2074 6865 2063 6f70  success, the cop
-00020b30: 6965 6420 6d65 7373 6167 6520 6973 2072  ied message is r
-00020b40: 6574 7572 6e65 642e 0a0a 2020 2020 2020  eturned...      
-00020b50: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-00020b60: 2020 2020 2020 5250 4345 7272 6f72 3a20        RPCError: 
-00020b70: 496e 2063 6173 6520 6f66 2061 2054 656c  In case of a Tel
-00020b80: 6567 7261 6d20 5250 4320 6572 726f 722e  egram RPC error.
-00020b90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00020ba0: 2020 2020 2069 6620 7365 6c66 2e73 6572       if self.ser
-00020bb0: 7669 6365 3a0a 2020 2020 2020 2020 2020  vice:.          
-00020bc0: 2020 6c6f 672e 7761 726e 696e 6728 6622    log.warning(f"
-00020bd0: 5365 7276 6963 6520 6d65 7373 6167 6573  Service messages
-00020be0: 2063 616e 6e6f 7420 6265 2063 6f70 6965   cannot be copie
-00020bf0: 642e 2022 0a20 2020 2020 2020 2020 2020  d. ".           
-00020c00: 2020 2020 2020 2020 2020 2020 2066 2263               f"c
-00020c10: 6861 745f 6964 3a20 7b73 656c 662e 6368  hat_id: {self.ch
-00020c20: 6174 2e69 647d 2c20 6d65 7373 6167 655f  at.id}, message_
-00020c30: 6964 3a20 7b73 656c 662e 6964 7d22 290a  id: {self.id}").
-00020c40: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-00020c50: 662e 6761 6d65 2061 6e64 206e 6f74 2061  f.game and not a
-00020c60: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
-00020c70: 742e 7374 6f72 6167 652e 6973 5f62 6f74  t.storage.is_bot
-00020c80: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00020c90: 6c6f 672e 7761 726e 696e 6728 6622 5573  log.warning(f"Us
-00020ca0: 6572 7320 6361 6e6e 6f74 2073 656e 6420  ers cannot send 
-00020cb0: 6d65 7373 6167 6573 2077 6974 6820 4761  messages with Ga
-00020cc0: 6d65 206d 6564 6961 2074 7970 652e 2022  me media type. "
-00020cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020ce0: 2020 2020 2020 2020 2066 2263 6861 745f           f"chat_
-00020cf0: 6964 3a20 7b73 656c 662e 6368 6174 2e69  id: {self.chat.i
-00020d00: 647d 2c20 6d65 7373 6167 655f 6964 3a20  d}, message_id: 
-00020d10: 7b73 656c 662e 6964 7d22 290a 2020 2020  {self.id}").    
-00020d20: 2020 2020 656c 6966 2073 656c 662e 656d      elif self.em
-00020d30: 7074 793a 0a20 2020 2020 2020 2020 2020  pty:.           
-00020d40: 206c 6f67 2e77 6172 6e69 6e67 2866 2245   log.warning(f"E
-00020d50: 6d70 7479 206d 6573 7361 6765 7320 6361  mpty messages ca
-00020d60: 6e6e 6f74 2062 6520 636f 7069 6564 2e20  nnot be copied. 
-00020d70: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
-00020d80: 7365 6c66 2e74 6578 743a 0a20 2020 2020  self.text:.     
-00020d90: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-00020da0: 6169 7420 7365 6c66 2e5f 636c 6965 6e74  ait self._client
-00020db0: 2e73 656e 645f 6d65 7373 6167 6528 0a20  .send_message(. 
-00020dc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00020dd0: 6861 745f 6964 2c0a 2020 2020 2020 2020  hat_id,.        
-00020de0: 2020 2020 2020 2020 7465 7874 3d73 656c          text=sel
-00020df0: 662e 7465 7874 2c0a 2020 2020 2020 2020  f.text,.        
-00020e00: 2020 2020 2020 2020 656e 7469 7469 6573          entities
-00020e10: 3d73 656c 662e 656e 7469 7469 6573 2c0a  =self.entities,.
-00020e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e30: 7061 7273 655f 6d6f 6465 3d65 6e75 6d73  parse_mode=enums
-00020e40: 2e50 6172 7365 4d6f 6465 2e44 4953 4142  .ParseMode.DISAB
-00020e50: 4c45 442c 0a20 2020 2020 2020 2020 2020  LED,.           
-00020e60: 2020 2020 2064 6973 6162 6c65 5f77 6562       disable_web
-00020e70: 5f70 6167 655f 7072 6576 6965 773d 6e6f  _page_preview=no
-00020e80: 7420 7365 6c66 2e77 6562 5f70 6167 652c  t self.web_page,
-00020e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020ea0: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-00020eb0: 6174 696f 6e3d 6469 7361 626c 655f 6e6f  ation=disable_no
-00020ec0: 7469 6669 6361 7469 6f6e 2c0a 2020 2020  tification,.    
-00020ed0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00020ee0: 6167 655f 7468 7265 6164 5f69 643d 6d65  age_thread_id=me
-00020ef0: 7373 6167 655f 7468 7265 6164 5f69 642c  ssage_thread_id,
-00020f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020f10: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
-00020f20: 655f 6964 3d72 6570 6c79 5f74 6f5f 6d65  e_id=reply_to_me
-00020f30: 7373 6167 655f 6964 2c0a 2020 2020 2020  ssage_id,.      
-00020f40: 2020 2020 2020 2020 2020 7363 6865 6475            schedu
-00020f50: 6c65 5f64 6174 653d 7363 6865 6475 6c65  le_date=schedule
-00020f60: 5f64 6174 652c 0a20 2020 2020 2020 2020  _date,.         
-00020f70: 2020 2020 2020 2070 726f 7465 6374 5f63         protect_c
-00020f80: 6f6e 7465 6e74 3d70 726f 7465 6374 5f63  ontent=protect_c
-00020f90: 6f6e 7465 6e74 2c0a 2020 2020 2020 2020  ontent,.        
-00020fa0: 2020 2020 2020 2020 7265 706c 795f 6d61          reply_ma
-00020fb0: 726b 7570 3d73 656c 662e 7265 706c 795f  rkup=self.reply_
-00020fc0: 6d61 726b 7570 2069 6620 7265 706c 795f  markup if reply_
-00020fd0: 6d61 726b 7570 2069 7320 6f62 6a65 6374  markup is object
-00020fe0: 2065 6c73 6520 7265 706c 795f 6d61 726b   else reply_mark
-00020ff0: 7570 0a20 2020 2020 2020 2020 2020 2029  up.            )
-00021000: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
-00021010: 6c66 2e6d 6564 6961 3a0a 2020 2020 2020  lf.media:.      
-00021020: 2020 2020 2020 7365 6e64 5f6d 6564 6961        send_media
-00021030: 203d 2070 6172 7469 616c 280a 2020 2020   = partial(.    
-00021040: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00021050: 2e5f 636c 6965 6e74 2e73 656e 645f 6361  ._client.send_ca
-00021060: 6368 6564 5f6d 6564 6961 2c0a 2020 2020  ched_media,.    
-00021070: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-00021080: 5f69 643d 6368 6174 5f69 642c 0a20 2020  _id=chat_id,.   
-00021090: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-000210a0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-000210b0: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
-000210c0: 6361 7469 6f6e 2c0a 2020 2020 2020 2020  cation,.        
-000210d0: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
-000210e0: 7468 7265 6164 5f69 643d 6d65 7373 6167  thread_id=messag
-000210f0: 655f 7468 7265 6164 5f69 642c 0a20 2020  e_thread_id,.   
-00021100: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-00021110: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-00021120: 3d72 6570 6c79 5f74 6f5f 6d65 7373 6167  =reply_to_messag
-00021130: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
-00021140: 2020 2020 2020 7363 6865 6475 6c65 5f64        schedule_d
-00021150: 6174 653d 7363 6865 6475 6c65 5f64 6174  ate=schedule_dat
-00021160: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00021170: 2020 2070 726f 7465 6374 5f63 6f6e 7465     protect_conte
-00021180: 6e74 3d70 726f 7465 6374 5f63 6f6e 7465  nt=protect_conte
-00021190: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
-000211a0: 2020 2020 7265 706c 795f 6d61 726b 7570      reply_markup
-000211b0: 3d73 656c 662e 7265 706c 795f 6d61 726b  =self.reply_mark
-000211c0: 7570 2069 6620 7265 706c 795f 6d61 726b  up if reply_mark
-000211d0: 7570 2069 7320 6f62 6a65 6374 2065 6c73  up is object els
-000211e0: 6520 7265 706c 795f 6d61 726b 7570 0a20  e reply_markup. 
-000211f0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00021200: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00021210: 662e 7068 6f74 6f3a 0a20 2020 2020 2020  f.photo:.       
-00021220: 2020 2020 2020 2020 2066 696c 655f 6964           file_id
-00021230: 203d 2073 656c 662e 7068 6f74 6f2e 6669   = self.photo.fi
-00021240: 6c65 5f69 640a 2020 2020 2020 2020 2020  le_id.          
-00021250: 2020 656c 6966 2073 656c 662e 6175 6469    elif self.audi
-00021260: 6f3a 0a20 2020 2020 2020 2020 2020 2020  o:.             
-00021270: 2020 2066 696c 655f 6964 203d 2073 656c     file_id = sel
-00021280: 662e 6175 6469 6f2e 6669 6c65 5f69 640a  f.audio.file_id.
-00021290: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000212a0: 2073 656c 662e 646f 6375 6d65 6e74 3a0a   self.document:.
-000212b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000212c0: 6669 6c65 5f69 6420 3d20 7365 6c66 2e64  file_id = self.d
-000212d0: 6f63 756d 656e 742e 6669 6c65 5f69 640a  ocument.file_id.
-000212e0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000212f0: 2073 656c 662e 7669 6465 6f3a 0a20 2020   self.video:.   
-00021300: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00021310: 655f 6964 203d 2073 656c 662e 7669 6465  e_id = self.vide
-00021320: 6f2e 6669 6c65 5f69 640a 2020 2020 2020  o.file_id.      
-00021330: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-00021340: 616e 696d 6174 696f 6e3a 0a20 2020 2020  animation:.     
-00021350: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-00021360: 6964 203d 2073 656c 662e 616e 696d 6174  id = self.animat
-00021370: 696f 6e2e 6669 6c65 5f69 640a 2020 2020  ion.file_id.    
-00021380: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-00021390: 662e 766f 6963 653a 0a20 2020 2020 2020  f.voice:.       
-000213a0: 2020 2020 2020 2020 2066 696c 655f 6964           file_id
-000213b0: 203d 2073 656c 662e 766f 6963 652e 6669   = self.voice.fi
-000213c0: 6c65 5f69 640a 2020 2020 2020 2020 2020  le_id.          
-000213d0: 2020 656c 6966 2073 656c 662e 7374 6963    elif self.stic
-000213e0: 6b65 723a 0a20 2020 2020 2020 2020 2020  ker:.           
-000213f0: 2020 2020 2066 696c 655f 6964 203d 2073       file_id = s
-00021400: 656c 662e 7374 6963 6b65 722e 6669 6c65  elf.sticker.file
-00021410: 5f69 640a 2020 2020 2020 2020 2020 2020  _id.            
-00021420: 656c 6966 2073 656c 662e 7669 6465 6f5f  elif self.video_
-00021430: 6e6f 7465 3a0a 2020 2020 2020 2020 2020  note:.          
-00021440: 2020 2020 2020 6669 6c65 5f69 6420 3d20        file_id = 
-00021450: 7365 6c66 2e76 6964 656f 5f6e 6f74 652e  self.video_note.
-00021460: 6669 6c65 5f69 640a 2020 2020 2020 2020  file_id.        
-00021470: 2020 2020 656c 6966 2073 656c 662e 636f      elif self.co
-00021480: 6e74 6163 743a 0a20 2020 2020 2020 2020  ntact:.         
-00021490: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-000214a0: 6169 7420 7365 6c66 2e5f 636c 6965 6e74  ait self._client
-000214b0: 2e73 656e 645f 636f 6e74 6163 7428 0a20  .send_contact(. 
-000214c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000214d0: 2020 2063 6861 745f 6964 2c0a 2020 2020     chat_id,.    
-000214e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000214f0: 7068 6f6e 655f 6e75 6d62 6572 3d73 656c  phone_number=sel
-00021500: 662e 636f 6e74 6163 742e 7068 6f6e 655f  f.contact.phone_
-00021510: 6e75 6d62 6572 2c0a 2020 2020 2020 2020  number,.        
-00021520: 2020 2020 2020 2020 2020 2020 6669 7273              firs
-00021530: 745f 6e61 6d65 3d73 656c 662e 636f 6e74  t_name=self.cont
-00021540: 6163 742e 6669 7273 745f 6e61 6d65 2c0a  act.first_name,.
-00021550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021560: 2020 2020 6c61 7374 5f6e 616d 653d 7365      last_name=se
-00021570: 6c66 2e63 6f6e 7461 6374 2e6c 6173 745f  lf.contact.last_
-00021580: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-00021590: 2020 2020 2020 2020 2020 7663 6172 643d            vcard=
-000215a0: 7365 6c66 2e63 6f6e 7461 6374 2e76 6361  self.contact.vca
-000215b0: 7264 2c0a 2020 2020 2020 2020 2020 2020  rd,.            
-000215c0: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
-000215d0: 6e6f 7469 6669 6361 7469 6f6e 3d64 6973  notification=dis
-000215e0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-000215f0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00021600: 2020 2020 2020 206d 6573 7361 6765 5f74         message_t
-00021610: 6872 6561 645f 6964 3d6d 6573 7361 6765  hread_id=message
-00021620: 5f74 6872 6561 645f 6964 2c0a 2020 2020  _thread_id,.    
-00021630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021640: 7363 6865 6475 6c65 5f64 6174 653d 7363  schedule_date=sc
-00021650: 6865 6475 6c65 5f64 6174 650a 2020 2020  hedule_date.    
-00021660: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00021670: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
-00021680: 656c 662e 6c6f 6361 7469 6f6e 3a0a 2020  elf.location:.  
-00021690: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000216a0: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-000216b0: 5f63 6c69 656e 742e 7365 6e64 5f6c 6f63  _client.send_loc
-000216c0: 6174 696f 6e28 0a20 2020 2020 2020 2020  ation(.         
-000216d0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-000216e0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-000216f0: 2020 2020 2020 2020 6c61 7469 7475 6465          latitude
-00021700: 3d73 656c 662e 6c6f 6361 7469 6f6e 2e6c  =self.location.l
-00021710: 6174 6974 7564 652c 0a20 2020 2020 2020  atitude,.       
-00021720: 2020 2020 2020 2020 2020 2020 206c 6f6e               lon
-00021730: 6769 7475 6465 3d73 656c 662e 6c6f 6361  gitude=self.loca
-00021740: 7469 6f6e 2e6c 6f6e 6769 7475 6465 2c0a  tion.longitude,.
+0001f6f0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0001f700: 2070 726f 7465 6374 5f63 6f6e 7465 6e74   protect_content
+0001f710: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+0001f720: 2020 2020 2020 2064 726f 705f 6175 7468         drop_auth
+0001f730: 6f72 3a20 626f 6f6c 203d 204e 6f6e 650a  or: bool = None.
+0001f740: 2020 2020 2920 2d3e 2055 6e69 6f6e 5b22      ) -> Union["
+0001f750: 7479 7065 732e 4d65 7373 6167 6522 2c20  types.Message", 
+0001f760: 4c69 7374 5b22 7479 7065 732e 4d65 7373  List["types.Mess
+0001f770: 6167 6522 5d5d 3a0a 2020 2020 2020 2020  age"]]:.        
+0001f780: 2222 2242 6f75 6e64 206d 6574 686f 6420  """Bound method 
+0001f790: 2a66 6f72 7761 7264 2a20 6f66 203a 6f62  *forward* of :ob
+0001f7a0: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
+0001f7b0: 6573 2e4d 6573 7361 6765 602e 0a0a 2020  es.Message`...  
+0001f7c0: 2020 2020 2020 5573 6520 6173 2061 2073        Use as a s
+0001f7d0: 686f 7274 6375 7420 666f 723a 0a0a 2020  hortcut for:..  
+0001f7e0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+0001f7f0: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+0001f800: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+0001f810: 636c 6965 6e74 2e66 6f72 7761 7264 5f6d  client.forward_m
+0001f820: 6573 7361 6765 7328 0a20 2020 2020 2020  essages(.       
+0001f830: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+0001f840: 3d63 6861 745f 6964 2c0a 2020 2020 2020  =chat_id,.      
+0001f850: 2020 2020 2020 2020 2020 6672 6f6d 5f63            from_c
+0001f860: 6861 745f 6964 3d6d 6573 7361 6765 2e63  hat_id=message.c
+0001f870: 6861 742e 6964 2c0a 2020 2020 2020 2020  hat.id,.        
+0001f880: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+0001f890: 6964 733d 6d65 7373 6167 652e 6964 0a20  ids=message.id. 
+0001f8a0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0001f8b0: 2020 2020 2020 4578 616d 706c 653a 0a20        Example:. 
+0001f8c0: 2020 2020 2020 2020 2020 202e 2e20 636f             .. co
+0001f8d0: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
+0001f8e0: 6e0a 0a20 2020 2020 2020 2020 2020 2020  n..             
+0001f8f0: 2020 2061 7761 6974 206d 6573 7361 6765     await message
+0001f900: 2e66 6f72 7761 7264 2863 6861 745f 6964  .forward(chat_id
+0001f910: 290a 0a20 2020 2020 2020 2050 6172 616d  )..        Param
+0001f920: 6574 6572 733a 0a20 2020 2020 2020 2020  eters:.         
+0001f930: 2020 2063 6861 745f 6964 2028 6060 696e     chat_id (``in
+0001f940: 7460 6020 7c20 6060 7374 7260 6029 3a0a  t`` | ``str``):.
+0001f950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f960: 556e 6971 7565 2069 6465 6e74 6966 6965  Unique identifie
+0001f970: 7220 2869 6e74 2920 6f72 2075 7365 726e  r (int) or usern
+0001f980: 616d 6520 2873 7472 2920 6f66 2074 6865  ame (str) of the
+0001f990: 2074 6172 6765 7420 6368 6174 2e0a 2020   target chat..  
+0001f9a0: 2020 2020 2020 2020 2020 2020 2020 466f                Fo
+0001f9b0: 7220 796f 7572 2070 6572 736f 6e61 6c20  r your personal 
+0001f9c0: 636c 6f75 6420 2853 6176 6564 204d 6573  cloud (Saved Mes
+0001f9d0: 7361 6765 7329 2079 6f75 2063 616e 2073  sages) you can s
+0001f9e0: 696d 706c 7920 7573 6520 226d 6522 206f  imply use "me" o
+0001f9f0: 7220 2273 656c 6622 2e0a 2020 2020 2020  r "self"..      
+0001fa00: 2020 2020 2020 2020 2020 466f 7220 6120            For a 
+0001fa10: 636f 6e74 6163 7420 7468 6174 2065 7869  contact that exi
+0001fa20: 7374 7320 696e 2079 6f75 7220 5465 6c65  sts in your Tele
+0001fa30: 6772 616d 2061 6464 7265 7373 2062 6f6f  gram address boo
+0001fa40: 6b20 796f 7520 6361 6e20 7573 6520 6869  k you can use hi
+0001fa50: 7320 7068 6f6e 6520 6e75 6d62 6572 2028  s phone number (
+0001fa60: 7374 7229 2e0a 0a20 2020 2020 2020 2020  str)...         
+0001fa70: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
+0001fa80: 645f 6964 2028 6060 696e 7460 602c 202a  d_id (``int``, *
+0001fa90: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
+0001faa0: 2020 2020 2020 2020 2020 2020 556e 6971              Uniq
+0001fab0: 7565 2069 6465 6e74 6966 6965 7220 6f66  ue identifier of
+0001fac0: 2061 206d 6573 7361 6765 2074 6872 6561   a message threa
+0001fad0: 6420 746f 2077 6869 6368 2074 6865 206d  d to which the m
+0001fae0: 6573 7361 6765 2062 656c 6f6e 6773 3b20  essage belongs; 
+0001faf0: 666f 7220 7375 7065 7267 726f 7570 7320  for supergroups 
+0001fb00: 6f6e 6c79 0a0a 2020 2020 2020 2020 2020  only..          
+0001fb10: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
+0001fb20: 6361 7469 6f6e 2028 6060 626f 6f6c 6060  cation (``bool``
+0001fb30: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
+0001fb40: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0001fb50: 656e 6473 2074 6865 206d 6573 7361 6765  ends the message
+0001fb60: 2073 696c 656e 746c 792e 0a20 2020 2020   silently..     
+0001fb70: 2020 2020 2020 2020 2020 2055 7365 7273             Users
+0001fb80: 2077 696c 6c20 7265 6365 6976 6520 6120   will receive a 
+0001fb90: 6e6f 7469 6669 6361 7469 6f6e 2077 6974  notification wit
+0001fba0: 6820 6e6f 2073 6f75 6e64 2e0a 0a20 2020  h no sound...   
+0001fbb0: 2020 2020 2020 2020 2073 6368 6564 756c           schedul
+0001fbc0: 655f 6461 7465 2028 3a70 793a 6f62 6a3a  e_date (:py:obj:
+0001fbd0: 607e 6461 7465 7469 6d65 2e64 6174 6574  `~datetime.datet
+0001fbe0: 696d 6560 2c20 2a6f 7074 696f 6e61 6c2a  ime`, *optional*
+0001fbf0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001fc00: 2020 2044 6174 6520 7768 656e 2074 6865     Date when the
+0001fc10: 206d 6573 7361 6765 2077 696c 6c20 6265   message will be
+0001fc20: 2061 7574 6f6d 6174 6963 616c 6c79 2073   automatically s
+0001fc30: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
+0001fc40: 2020 7072 6f74 6563 745f 636f 6e74 656e    protect_conten
+0001fc50: 7420 2860 6062 6f6f 6c60 602c 202a 6f70  t (``bool``, *op
+0001fc60: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
+0001fc70: 2020 2020 2020 2020 2020 5072 6f74 6563            Protec
+0001fc80: 7473 2074 6865 2063 6f6e 7465 6e74 7320  ts the contents 
+0001fc90: 6f66 2074 6865 2073 656e 7420 6d65 7373  of the sent mess
+0001fca0: 6167 6520 6672 6f6d 2066 6f72 7761 7264  age from forward
+0001fcb0: 696e 6720 616e 6420 7361 7669 6e67 2e0a  ing and saving..
+0001fcc0: 0a20 2020 2020 2020 2020 2020 2064 726f  .            dro
+0001fcd0: 705f 6175 7468 6f72 2028 6060 626f 6f6c  p_author (``bool
+0001fce0: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+0001fcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fd00: 2046 6f72 7761 7264 7320 6d65 7373 6167   Forwards messag
+0001fd10: 6573 2077 6974 686f 7574 2071 756f 7469  es without quoti
+0001fd20: 6e67 2074 6865 206f 7269 6769 6e61 6c20  ng the original 
+0001fd30: 6175 7468 6f72 0a0a 2020 2020 2020 2020  author..        
+0001fd40: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0001fd50: 2020 2020 204f 6e20 7375 6363 6573 732c       On success,
+0001fd60: 2074 6865 2066 6f72 7761 7264 6564 204d   the forwarded M
+0001fd70: 6573 7361 6765 2069 7320 7265 7475 726e  essage is return
+0001fd80: 6564 2e0a 0a20 2020 2020 2020 2052 6169  ed...        Rai
+0001fd90: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+0001fda0: 2052 5043 4572 726f 723a 2049 6e20 6361   RPCError: In ca
+0001fdb0: 7365 206f 6620 6120 5465 6c65 6772 616d  se of a Telegram
+0001fdc0: 2052 5043 2065 7272 6f72 2e0a 2020 2020   RPC error..    
+0001fdd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0001fde0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+0001fdf0: 662e 5f63 6c69 656e 742e 666f 7277 6172  f._client.forwar
+0001fe00: 645f 6d65 7373 6167 6573 280a 2020 2020  d_messages(.    
+0001fe10: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+0001fe20: 6368 6174 5f69 642c 0a20 2020 2020 2020  chat_id,.       
+0001fe30: 2020 2020 2066 726f 6d5f 6368 6174 5f69       from_chat_i
+0001fe40: 643d 7365 6c66 2e63 6861 742e 6964 2c0a  d=self.chat.id,.
+0001fe50: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
+0001fe60: 6167 655f 6964 733d 7365 6c66 2e69 642c  age_ids=self.id,
+0001fe70: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
+0001fe80: 7361 6765 5f74 6872 6561 645f 6964 3d6d  sage_thread_id=m
+0001fe90: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+0001fea0: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+0001feb0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+0001fec0: 6f6e 3d64 6973 6162 6c65 5f6e 6f74 6966  on=disable_notif
+0001fed0: 6963 6174 696f 6e2c 0a20 2020 2020 2020  ication,.       
+0001fee0: 2020 2020 2073 6368 6564 756c 655f 6461       schedule_da
+0001fef0: 7465 3d73 6368 6564 756c 655f 6461 7465  te=schedule_date
+0001ff00: 2c0a 2020 2020 2020 2020 2020 2020 7072  ,.            pr
+0001ff10: 6f74 6563 745f 636f 6e74 656e 743d 7072  otect_content=pr
+0001ff20: 6f74 6563 745f 636f 6e74 656e 742c 0a20  otect_content,. 
+0001ff30: 2020 2020 2020 2020 2020 2064 726f 705f             drop_
+0001ff40: 6175 7468 6f72 3d64 726f 705f 6175 7468  author=drop_auth
+0001ff50: 6f72 0a20 2020 2020 2020 2029 0a0a 2020  or.        )..  
+0001ff60: 2020 6173 796e 6320 6465 6620 636f 7079    async def copy
+0001ff70: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0001ff80: 2020 2020 2020 2020 6368 6174 5f69 643a          chat_id:
+0001ff90: 2055 6e69 6f6e 5b69 6e74 2c20 7374 725d   Union[int, str]
+0001ffa0: 2c0a 2020 2020 2020 2020 6361 7074 696f  ,.        captio
+0001ffb0: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
+0001ffc0: 2020 2020 2020 2070 6172 7365 5f6d 6f64         parse_mod
+0001ffd0: 653a 204f 7074 696f 6e61 6c5b 2265 6e75  e: Optional["enu
+0001ffe0: 6d73 2e50 6172 7365 4d6f 6465 225d 203d  ms.ParseMode"] =
+0001fff0: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
+00020000: 6170 7469 6f6e 5f65 6e74 6974 6965 733a  aption_entities:
+00020010: 204c 6973 745b 2274 7970 6573 2e4d 6573   List["types.Mes
+00020020: 7361 6765 456e 7469 7479 225d 203d 204e  sageEntity"] = N
+00020030: 6f6e 652c 0a20 2020 2020 2020 2064 6973  one,.        dis
+00020040: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00020050: 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  n: bool = None,.
+00020060: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+00020070: 7468 7265 6164 5f69 643a 2069 6e74 203d  thread_id: int =
+00020080: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
+00020090: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+000200a0: 6964 3a20 696e 7420 3d20 4e6f 6e65 2c0a  id: int = None,.
+000200b0: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
+000200c0: 5f64 6174 653a 2064 6174 6574 696d 6520  _date: datetime 
+000200d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000200e0: 7072 6f74 6563 745f 636f 6e74 656e 743a  protect_content:
+000200f0: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
+00020100: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
+00020110: 7570 3a20 556e 696f 6e5b 0a20 2020 2020  up: Union[.     
+00020120: 2020 2020 2020 2022 7479 7065 732e 496e         "types.In
+00020130: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
+00020140: 7570 222c 0a20 2020 2020 2020 2020 2020  up",.           
+00020150: 2022 7479 7065 732e 5265 706c 794b 6579   "types.ReplyKey
+00020160: 626f 6172 644d 6172 6b75 7022 2c0a 2020  boardMarkup",.  
+00020170: 2020 2020 2020 2020 2020 2274 7970 6573            "types
+00020180: 2e52 6570 6c79 4b65 7962 6f61 7264 5265  .ReplyKeyboardRe
+00020190: 6d6f 7665 222c 0a20 2020 2020 2020 2020  move",.         
+000201a0: 2020 2022 7479 7065 732e 466f 7263 6552     "types.ForceR
+000201b0: 6570 6c79 220a 2020 2020 2020 2020 5d20  eply".        ] 
+000201c0: 3d20 6f62 6a65 6374 0a20 2020 2029 202d  = object.    ) -
+000201d0: 3e20 556e 696f 6e5b 2274 7970 6573 2e4d  > Union["types.M
+000201e0: 6573 7361 6765 222c 204c 6973 745b 2274  essage", List["t
+000201f0: 7970 6573 2e4d 6573 7361 6765 225d 5d3a  ypes.Message"]]:
+00020200: 0a20 2020 2020 2020 2022 2222 426f 756e  .        """Boun
+00020210: 6420 6d65 7468 6f64 202a 636f 7079 2a20  d method *copy* 
+00020220: 6f66 203a 6f62 6a3a 607e 7079 726f 6772  of :obj:`~pyrogr
+00020230: 616d 2e74 7970 6573 2e4d 6573 7361 6765  am.types.Message
+00020240: 602e 0a0a 2020 2020 2020 2020 5573 6520  `...        Use 
+00020250: 6173 2061 2073 686f 7274 6375 7420 666f  as a shortcut fo
+00020260: 723a 0a0a 2020 2020 2020 2020 2e2e 2063  r:..        .. c
+00020270: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00020280: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+00020290: 6177 6169 7420 636c 6965 6e74 2e63 6f70  await client.cop
+000202a0: 795f 6d65 7373 6167 6528 0a20 2020 2020  y_message(.     
+000202b0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+000202c0: 6964 3d63 6861 745f 6964 2c0a 2020 2020  id=chat_id,.    
+000202d0: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
+000202e0: 5f63 6861 745f 6964 3d6d 6573 7361 6765  _chat_id=message
+000202f0: 2e63 6861 742e 6964 2c0a 2020 2020 2020  .chat.id,.      
+00020300: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00020310: 655f 6964 3d6d 6573 7361 6765 2e69 640a  e_id=message.id.
+00020320: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00020330: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
+00020340: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
+00020350: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00020360: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+00020370: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
+00020380: 652e 636f 7079 2863 6861 745f 6964 290a  e.copy(chat_id).
+00020390: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+000203a0: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+000203b0: 2063 6861 745f 6964 2028 6060 696e 7460   chat_id (``int`
+000203c0: 6020 7c20 6060 7374 7260 6029 3a0a 2020  ` | ``str``):.  
+000203d0: 2020 2020 2020 2020 2020 2020 2020 556e                Un
+000203e0: 6971 7565 2069 6465 6e74 6966 6965 7220  ique identifier 
+000203f0: 2869 6e74 2920 6f72 2075 7365 726e 616d  (int) or usernam
+00020400: 6520 2873 7472 2920 6f66 2074 6865 2074  e (str) of the t
+00020410: 6172 6765 7420 6368 6174 2e0a 2020 2020  arget chat..    
+00020420: 2020 2020 2020 2020 2020 2020 466f 7220              For 
+00020430: 796f 7572 2070 6572 736f 6e61 6c20 636c  your personal cl
+00020440: 6f75 6420 2853 6176 6564 204d 6573 7361  oud (Saved Messa
+00020450: 6765 7329 2079 6f75 2063 616e 2073 696d  ges) you can sim
+00020460: 706c 7920 7573 6520 226d 6522 206f 7220  ply use "me" or 
+00020470: 2273 656c 6622 2e0a 2020 2020 2020 2020  "self"..        
+00020480: 2020 2020 2020 2020 466f 7220 6120 636f          For a co
+00020490: 6e74 6163 7420 7468 6174 2065 7869 7374  ntact that exist
+000204a0: 7320 696e 2079 6f75 7220 5465 6c65 6772  s in your Telegr
+000204b0: 616d 2061 6464 7265 7373 2062 6f6f 6b20  am address book 
+000204c0: 796f 7520 6361 6e20 7573 6520 6869 7320  you can use his 
+000204d0: 7068 6f6e 6520 6e75 6d62 6572 2028 7374  phone number (st
+000204e0: 7229 2e0a 0a20 2020 2020 2020 2020 2020  r)...           
+000204f0: 2063 6170 7469 6f6e 2028 6060 7374 7269   caption (``stri
+00020500: 6e67 6060 2c20 2a6f 7074 696f 6e61 6c2a  ng``, *optional*
+00020510: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00020520: 2020 204e 6577 2063 6170 7469 6f6e 2066     New caption f
+00020530: 6f72 206d 6564 6961 2c20 302d 3130 3234  or media, 0-1024
+00020540: 2063 6861 7261 6374 6572 7320 6166 7465   characters afte
+00020550: 7220 656e 7469 7469 6573 2070 6172 7369  r entities parsi
+00020560: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
+00020570: 2020 2020 4966 206e 6f74 2073 7065 6369      If not speci
+00020580: 6669 6564 2c20 7468 6520 6f72 6967 696e  fied, the origin
+00020590: 616c 2063 6170 7469 6f6e 2069 7320 6b65  al caption is ke
+000205a0: 7074 2e0a 2020 2020 2020 2020 2020 2020  pt..            
+000205b0: 2020 2020 5061 7373 2022 2220 2865 6d70      Pass "" (emp
+000205c0: 7479 2073 7472 696e 6729 2074 6f20 7265  ty string) to re
+000205d0: 6d6f 7665 2074 6865 2063 6170 7469 6f6e  move the caption
+000205e0: 2e0a 0a20 2020 2020 2020 2020 2020 2070  ...            p
+000205f0: 6172 7365 5f6d 6f64 6520 283a 6f62 6a3a  arse_mode (:obj:
+00020600: 607e 7079 726f 6772 616d 2e65 6e75 6d73  `~pyrogram.enums
+00020610: 2e50 6172 7365 4d6f 6465 602c 202a 6f70  .ParseMode`, *op
+00020620: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
+00020630: 2020 2020 2020 2020 2020 4279 2064 6566            By def
+00020640: 6175 6c74 2c20 7465 7874 7320 6172 6520  ault, texts are 
+00020650: 7061 7273 6564 2075 7369 6e67 2062 6f74  parsed using bot
+00020660: 6820 4d61 726b 646f 776e 2061 6e64 2048  h Markdown and H
+00020670: 544d 4c20 7374 796c 6573 2e0a 2020 2020  TML styles..    
+00020680: 2020 2020 2020 2020 2020 2020 596f 7520              You 
+00020690: 6361 6e20 636f 6d62 696e 6520 626f 7468  can combine both
+000206a0: 2073 796e 7461 7865 7320 746f 6765 7468   syntaxes togeth
+000206b0: 6572 2e0a 0a20 2020 2020 2020 2020 2020  er...           
+000206c0: 2063 6170 7469 6f6e 5f65 6e74 6974 6965   caption_entitie
+000206d0: 7320 284c 6973 7420 6f66 203a 6f62 6a3a  s (List of :obj:
+000206e0: 607e 7079 726f 6772 616d 2e74 7970 6573  `~pyrogram.types
+000206f0: 2e4d 6573 7361 6765 456e 7469 7479 6029  .MessageEntity`)
+00020700: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00020710: 2020 4c69 7374 206f 6620 7370 6563 6961    List of specia
+00020720: 6c20 656e 7469 7469 6573 2074 6861 7420  l entities that 
+00020730: 6170 7065 6172 2069 6e20 7468 6520 6e65  appear in the ne
+00020740: 7720 6361 7074 696f 6e2c 2077 6869 6368  w caption, which
+00020750: 2063 616e 2062 6520 7370 6563 6966 6965   can be specifie
+00020760: 6420 696e 7374 6561 6420 6f66 202a 7061  d instead of *pa
+00020770: 7273 655f 6d6f 6465 2a2e 0a0a 2020 2020  rse_mode*...    
+00020780: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
+00020790: 6e6f 7469 6669 6361 7469 6f6e 2028 6060  notification (``
+000207a0: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
+000207b0: 6c2a 293a 0a20 2020 2020 2020 2020 2020  l*):.           
+000207c0: 2020 2020 2053 656e 6473 2074 6865 206d       Sends the m
+000207d0: 6573 7361 6765 2073 696c 656e 746c 792e  essage silently.
+000207e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000207f0: 2055 7365 7273 2077 696c 6c20 7265 6365   Users will rece
+00020800: 6976 6520 6120 6e6f 7469 6669 6361 7469  ive a notificati
+00020810: 6f6e 2077 6974 6820 6e6f 2073 6f75 6e64  on with no sound
+00020820: 2e0a 0a20 2020 2020 2020 2020 2020 206d  ...            m
+00020830: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+00020840: 2028 6060 696e 7460 602c 202a 6f70 7469   (``int``, *opti
+00020850: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
+00020860: 2020 2020 2020 2020 556e 6971 7565 2069          Unique i
+00020870: 6465 6e74 6966 6965 7220 666f 7220 7468  dentifier for th
+00020880: 6520 7461 7267 6574 206d 6573 7361 6765  e target message
+00020890: 2074 6872 6561 6420 2874 6f70 6963 2920   thread (topic) 
+000208a0: 6f66 2074 6865 2066 6f72 756d 2e0a 2020  of the forum..  
+000208b0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000208c0: 7220 666f 7275 6d20 7375 7065 7267 726f  r forum supergro
+000208d0: 7570 7320 6f6e 6c79 2e0a 0a20 2020 2020  ups only...     
+000208e0: 2020 2020 2020 2072 6570 6c79 5f74 6f5f         reply_to_
+000208f0: 6d65 7373 6167 655f 6964 2028 6060 696e  message_id (``in
+00020900: 7460 602c 202a 6f70 7469 6f6e 616c 2a29  t``, *optional*)
+00020910: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00020920: 2020 4966 2074 6865 206d 6573 7361 6765    If the message
+00020930: 2069 7320 6120 7265 706c 792c 2049 4420   is a reply, ID 
+00020940: 6f66 2074 6865 206f 7269 6769 6e61 6c20  of the original 
+00020950: 6d65 7373 6167 652e 0a0a 2020 2020 2020  message...      
+00020960: 2020 2020 2020 7363 6865 6475 6c65 5f64        schedule_d
+00020970: 6174 6520 283a 7079 3a6f 626a 3a60 7e64  ate (:py:obj:`~d
+00020980: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+00020990: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+000209a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000209b0: 4461 7465 2077 6865 6e20 7468 6520 6d65  Date when the me
+000209c0: 7373 6167 6520 7769 6c6c 2062 6520 6175  ssage will be au
+000209d0: 746f 6d61 7469 6361 6c6c 7920 7365 6e74  tomatically sent
+000209e0: 2e0a 0a20 2020 2020 2020 2020 2020 2070  ...            p
+000209f0: 726f 7465 6374 5f63 6f6e 7465 6e74 2028  rotect_content (
+00020a00: 6060 626f 6f6c 6060 2c20 2a6f 7074 696f  ``bool``, *optio
+00020a10: 6e61 6c2a 293a 0a20 2020 2020 2020 2020  nal*):.         
+00020a20: 2020 2020 2020 2050 726f 7465 6374 7320         Protects 
+00020a30: 7468 6520 636f 6e74 656e 7473 206f 6620  the contents of 
+00020a40: 7468 6520 7365 6e74 206d 6573 7361 6765  the sent message
+00020a50: 2066 726f 6d20 666f 7277 6172 6469 6e67   from forwarding
+00020a60: 2061 6e64 2073 6176 696e 672e 0a0a 2020   and saving...  
+00020a70: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00020a80: 6d61 726b 7570 2028 3a6f 626a 3a60 7e70  markup (:obj:`~p
+00020a90: 7972 6f67 7261 6d2e 7479 7065 732e 496e  yrogram.types.In
+00020aa0: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
+00020ab0: 7570 6020 7c20 3a6f 626a 3a60 7e70 7972  up` | :obj:`~pyr
+00020ac0: 6f67 7261 6d2e 7479 7065 732e 5265 706c  ogram.types.Repl
+00020ad0: 794b 6579 626f 6172 644d 6172 6b75 7060  yKeyboardMarkup`
+00020ae0: 207c 203a 6f62 6a3a 607e 7079 726f 6772   | :obj:`~pyrogr
+00020af0: 616d 2e74 7970 6573 2e52 6570 6c79 4b65  am.types.ReplyKe
+00020b00: 7962 6f61 7264 5265 6d6f 7665 6020 7c20  yboardRemove` | 
+00020b10: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+00020b20: 7479 7065 732e 466f 7263 6552 6570 6c79  types.ForceReply
+00020b30: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+00020b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b50: 4164 6469 7469 6f6e 616c 2069 6e74 6572  Additional inter
+00020b60: 6661 6365 206f 7074 696f 6e73 2e20 416e  face options. An
+00020b70: 206f 626a 6563 7420 666f 7220 616e 2069   object for an i
+00020b80: 6e6c 696e 6520 6b65 7962 6f61 7264 2c20  nline keyboard, 
+00020b90: 6375 7374 6f6d 2072 6570 6c79 206b 6579  custom reply key
+00020ba0: 626f 6172 642c 0a20 2020 2020 2020 2020  board,.         
+00020bb0: 2020 2020 2020 2069 6e73 7472 7563 7469         instructi
+00020bc0: 6f6e 7320 746f 2072 656d 6f76 6520 7265  ons to remove re
+00020bd0: 706c 7920 6b65 7962 6f61 7264 206f 7220  ply keyboard or 
+00020be0: 746f 2066 6f72 6365 2061 2072 6570 6c79  to force a reply
+00020bf0: 2066 726f 6d20 7468 6520 7573 6572 2e0a   from the user..
+00020c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c10: 4966 206e 6f74 2073 7065 6369 6669 6564  If not specified
+00020c20: 2c20 7468 6520 6f72 6967 696e 616c 2072  , the original r
+00020c30: 6570 6c79 206d 6172 6b75 7020 6973 206b  eply markup is k
+00020c40: 6570 742e 0a20 2020 2020 2020 2020 2020  ept..           
+00020c50: 2020 2020 2050 6173 7320 4e6f 6e65 2074       Pass None t
+00020c60: 6f20 7265 6d6f 7665 2074 6865 2072 6570  o remove the rep
+00020c70: 6c79 206d 6172 6b75 702e 0a0a 2020 2020  ly markup...    
+00020c80: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00020c90: 2020 2020 2020 2020 203a 6f62 6a3a 607e           :obj:`~
+00020ca0: 7079 726f 6772 616d 2e74 7970 6573 2e4d  pyrogram.types.M
+00020cb0: 6573 7361 6765 603a 204f 6e20 7375 6363  essage`: On succ
+00020cc0: 6573 732c 2074 6865 2063 6f70 6965 6420  ess, the copied 
+00020cd0: 6d65 7373 6167 6520 6973 2072 6574 7572  message is retur
+00020ce0: 6e65 642e 0a0a 2020 2020 2020 2020 5261  ned...        Ra
+00020cf0: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
+00020d00: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
+00020d10: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
+00020d20: 6d20 5250 4320 6572 726f 722e 0a20 2020  m RPC error..   
+00020d30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00020d40: 2069 6620 7365 6c66 2e73 6572 7669 6365   if self.service
+00020d50: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00020d60: 672e 7761 726e 696e 6728 6622 5365 7276  g.warning(f"Serv
+00020d70: 6963 6520 6d65 7373 6167 6573 2063 616e  ice messages can
+00020d80: 6e6f 7420 6265 2063 6f70 6965 642e 2022  not be copied. "
+00020d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020da0: 2020 2020 2020 2020 2066 2263 6861 745f           f"chat_
+00020db0: 6964 3a20 7b73 656c 662e 6368 6174 2e69  id: {self.chat.i
+00020dc0: 647d 2c20 6d65 7373 6167 655f 6964 3a20  d}, message_id: 
+00020dd0: 7b73 656c 662e 6964 7d22 290a 2020 2020  {self.id}").    
+00020de0: 2020 2020 656c 6966 2073 656c 662e 6761      elif self.ga
+00020df0: 6d65 2061 6e64 206e 6f74 2061 7761 6974  me and not await
+00020e00: 2073 656c 662e 5f63 6c69 656e 742e 7374   self._client.st
+00020e10: 6f72 6167 652e 6973 5f62 6f74 2829 3a0a  orage.is_bot():.
+00020e20: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
+00020e30: 7761 726e 696e 6728 6622 5573 6572 7320  warning(f"Users 
+00020e40: 6361 6e6e 6f74 2073 656e 6420 6d65 7373  cannot send mess
+00020e50: 6167 6573 2077 6974 6820 4761 6d65 206d  ages with Game m
+00020e60: 6564 6961 2074 7970 652e 2022 0a20 2020  edia type. ".   
+00020e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e80: 2020 2020 2066 2263 6861 745f 6964 3a20       f"chat_id: 
+00020e90: 7b73 656c 662e 6368 6174 2e69 647d 2c20  {self.chat.id}, 
+00020ea0: 6d65 7373 6167 655f 6964 3a20 7b73 656c  message_id: {sel
+00020eb0: 662e 6964 7d22 290a 2020 2020 2020 2020  f.id}").        
+00020ec0: 656c 6966 2073 656c 662e 656d 7074 793a  elif self.empty:
+00020ed0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00020ee0: 2e77 6172 6e69 6e67 2866 2245 6d70 7479  .warning(f"Empty
+00020ef0: 206d 6573 7361 6765 7320 6361 6e6e 6f74   messages cannot
+00020f00: 2062 6520 636f 7069 6564 2e20 2229 0a20   be copied. "). 
+00020f10: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+00020f20: 2e74 6578 743a 0a20 2020 2020 2020 2020  .text:.         
+00020f30: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+00020f40: 7365 6c66 2e5f 636c 6965 6e74 2e73 656e  self._client.sen
+00020f50: 645f 6d65 7373 6167 6528 0a20 2020 2020  d_message(.     
+00020f60: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+00020f70: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00020f80: 2020 2020 7465 7874 3d73 656c 662e 7465      text=self.te
+00020f90: 7874 2c0a 2020 2020 2020 2020 2020 2020  xt,.            
+00020fa0: 2020 2020 656e 7469 7469 6573 3d73 656c      entities=sel
+00020fb0: 662e 656e 7469 7469 6573 2c0a 2020 2020  f.entities,.    
+00020fc0: 2020 2020 2020 2020 2020 2020 7061 7273              pars
+00020fd0: 655f 6d6f 6465 3d65 6e75 6d73 2e50 6172  e_mode=enums.Par
+00020fe0: 7365 4d6f 6465 2e44 4953 4142 4c45 442c  seMode.DISABLED,
+00020ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021000: 2064 6973 6162 6c65 5f77 6562 5f70 6167   disable_web_pag
+00021010: 655f 7072 6576 6965 773d 6e6f 7420 7365  e_preview=not se
+00021020: 6c66 2e77 6562 5f70 6167 652c 0a20 2020  lf.web_page,.   
+00021030: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00021040: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00021050: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
+00021060: 6361 7469 6f6e 2c0a 2020 2020 2020 2020  cation,.        
+00021070: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+00021080: 7468 7265 6164 5f69 643d 6d65 7373 6167  thread_id=messag
+00021090: 655f 7468 7265 6164 5f69 642c 0a20 2020  e_thread_id,.   
+000210a0: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+000210b0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+000210c0: 3d72 6570 6c79 5f74 6f5f 6d65 7373 6167  =reply_to_messag
+000210d0: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
+000210e0: 2020 2020 2020 7363 6865 6475 6c65 5f64        schedule_d
+000210f0: 6174 653d 7363 6865 6475 6c65 5f64 6174  ate=schedule_dat
+00021100: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00021110: 2020 2070 726f 7465 6374 5f63 6f6e 7465     protect_conte
+00021120: 6e74 3d70 726f 7465 6374 5f63 6f6e 7465  nt=protect_conte
+00021130: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+00021140: 2020 2020 7265 706c 795f 6d61 726b 7570      reply_markup
+00021150: 3d73 656c 662e 7265 706c 795f 6d61 726b  =self.reply_mark
+00021160: 7570 2069 6620 7265 706c 795f 6d61 726b  up if reply_mark
+00021170: 7570 2069 7320 6f62 6a65 6374 2065 6c73  up is object els
+00021180: 6520 7265 706c 795f 6d61 726b 7570 0a20  e reply_markup. 
+00021190: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000211a0: 2020 2020 2065 6c69 6620 7365 6c66 2e6d       elif self.m
+000211b0: 6564 6961 3a0a 2020 2020 2020 2020 2020  edia:.          
+000211c0: 2020 7365 6e64 5f6d 6564 6961 203d 2070    send_media = p
+000211d0: 6172 7469 616c 280a 2020 2020 2020 2020  artial(.        
+000211e0: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
+000211f0: 6965 6e74 2e73 656e 645f 6361 6368 6564  ient.send_cached
+00021200: 5f6d 6564 6961 2c0a 2020 2020 2020 2020  _media,.        
+00021210: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+00021220: 6368 6174 5f69 642c 0a20 2020 2020 2020  chat_id,.       
+00021230: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
+00021240: 5f6e 6f74 6966 6963 6174 696f 6e3d 6469  _notification=di
+00021250: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+00021260: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00021270: 2020 2020 6d65 7373 6167 655f 7468 7265      message_thre
+00021280: 6164 5f69 643d 6d65 7373 6167 655f 7468  ad_id=message_th
+00021290: 7265 6164 5f69 642c 0a20 2020 2020 2020  read_id,.       
+000212a0: 2020 2020 2020 2020 2072 6570 6c79 5f74           reply_t
+000212b0: 6f5f 6d65 7373 6167 655f 6964 3d72 6570  o_message_id=rep
+000212c0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+000212d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000212e0: 2020 7363 6865 6475 6c65 5f64 6174 653d    schedule_date=
+000212f0: 7363 6865 6475 6c65 5f64 6174 652c 0a20  schedule_date,. 
+00021300: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00021310: 726f 7465 6374 5f63 6f6e 7465 6e74 3d70  rotect_content=p
+00021320: 726f 7465 6374 5f63 6f6e 7465 6e74 2c0a  rotect_content,.
+00021330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021340: 7265 706c 795f 6d61 726b 7570 3d73 656c  reply_markup=sel
+00021350: 662e 7265 706c 795f 6d61 726b 7570 2069  f.reply_markup i
+00021360: 6620 7265 706c 795f 6d61 726b 7570 2069  f reply_markup i
+00021370: 7320 6f62 6a65 6374 2065 6c73 6520 7265  s object else re
+00021380: 706c 795f 6d61 726b 7570 0a20 2020 2020  ply_markup.     
+00021390: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000213a0: 2020 2020 2020 6966 2073 656c 662e 7068        if self.ph
+000213b0: 6f74 6f3a 0a20 2020 2020 2020 2020 2020  oto:.           
+000213c0: 2020 2020 2066 696c 655f 6964 203d 2073       file_id = s
+000213d0: 656c 662e 7068 6f74 6f2e 6669 6c65 5f69  elf.photo.file_i
+000213e0: 640a 2020 2020 2020 2020 2020 2020 656c  d.            el
+000213f0: 6966 2073 656c 662e 6175 6469 6f3a 0a20  if self.audio:. 
+00021400: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00021410: 696c 655f 6964 203d 2073 656c 662e 6175  ile_id = self.au
+00021420: 6469 6f2e 6669 6c65 5f69 640a 2020 2020  dio.file_id.    
+00021430: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+00021440: 662e 646f 6375 6d65 6e74 3a0a 2020 2020  f.document:.    
+00021450: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00021460: 5f69 6420 3d20 7365 6c66 2e64 6f63 756d  _id = self.docum
+00021470: 656e 742e 6669 6c65 5f69 640a 2020 2020  ent.file_id.    
+00021480: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+00021490: 662e 7669 6465 6f3a 0a20 2020 2020 2020  f.video:.       
+000214a0: 2020 2020 2020 2020 2066 696c 655f 6964           file_id
+000214b0: 203d 2073 656c 662e 7669 6465 6f2e 6669   = self.video.fi
+000214c0: 6c65 5f69 640a 2020 2020 2020 2020 2020  le_id.          
+000214d0: 2020 656c 6966 2073 656c 662e 616e 696d    elif self.anim
+000214e0: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
+000214f0: 2020 2020 2020 2066 696c 655f 6964 203d         file_id =
+00021500: 2073 656c 662e 616e 696d 6174 696f 6e2e   self.animation.
+00021510: 6669 6c65 5f69 640a 2020 2020 2020 2020  file_id.        
+00021520: 2020 2020 656c 6966 2073 656c 662e 766f      elif self.vo
+00021530: 6963 653a 0a20 2020 2020 2020 2020 2020  ice:.           
+00021540: 2020 2020 2066 696c 655f 6964 203d 2073       file_id = s
+00021550: 656c 662e 766f 6963 652e 6669 6c65 5f69  elf.voice.file_i
+00021560: 640a 2020 2020 2020 2020 2020 2020 656c  d.            el
+00021570: 6966 2073 656c 662e 7374 6963 6b65 723a  if self.sticker:
+00021580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021590: 2066 696c 655f 6964 203d 2073 656c 662e   file_id = self.
+000215a0: 7374 6963 6b65 722e 6669 6c65 5f69 640a  sticker.file_id.
+000215b0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000215c0: 2073 656c 662e 7669 6465 6f5f 6e6f 7465   self.video_note
+000215d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000215e0: 2020 6669 6c65 5f69 6420 3d20 7365 6c66    file_id = self
+000215f0: 2e76 6964 656f 5f6e 6f74 652e 6669 6c65  .video_note.file
+00021600: 5f69 640a 2020 2020 2020 2020 2020 2020  _id.            
+00021610: 656c 6966 2073 656c 662e 636f 6e74 6163  elif self.contac
+00021620: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00021630: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+00021640: 7365 6c66 2e5f 636c 6965 6e74 2e73 656e  self._client.sen
+00021650: 645f 636f 6e74 6163 7428 0a20 2020 2020  d_contact(.     
+00021660: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00021670: 6861 745f 6964 2c0a 2020 2020 2020 2020  hat_id,.        
+00021680: 2020 2020 2020 2020 2020 2020 7068 6f6e              phon
+00021690: 655f 6e75 6d62 6572 3d73 656c 662e 636f  e_number=self.co
+000216a0: 6e74 6163 742e 7068 6f6e 655f 6e75 6d62  ntact.phone_numb
+000216b0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+000216c0: 2020 2020 2020 2020 6669 7273 745f 6e61          first_na
+000216d0: 6d65 3d73 656c 662e 636f 6e74 6163 742e  me=self.contact.
+000216e0: 6669 7273 745f 6e61 6d65 2c0a 2020 2020  first_name,.    
+000216f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021700: 6c61 7374 5f6e 616d 653d 7365 6c66 2e63  last_name=self.c
+00021710: 6f6e 7461 6374 2e6c 6173 745f 6e61 6d65  ontact.last_name
+00021720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00021730: 2020 2020 2020 7663 6172 643d 7365 6c66        vcard=self
+00021740: 2e63 6f6e 7461 6374 2e76 6361 7264 2c0a  .contact.vcard,.
 00021750: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021760: 2020 2020 6469 7361 626c 655f 6e6f 7469      disable_noti
 00021770: 6669 6361 7469 6f6e 3d64 6973 6162 6c65  fication=disable
 00021780: 5f6e 6f74 6966 6963 6174 696f 6e2c 0a20  _notification,. 
 00021790: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000217a0: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
 000217b0: 645f 6964 3d6d 6573 7361 6765 5f74 6872  d_id=message_thr
 000217c0: 6561 645f 6964 2c0a 2020 2020 2020 2020  ead_id,.        
 000217d0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
 000217e0: 6475 6c65 5f64 6174 653d 7363 6865 6475  dule_date=schedu
 000217f0: 6c65 5f64 6174 650a 2020 2020 2020 2020  le_date.        
 00021800: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
 00021810: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-00021820: 7665 6e75 653a 0a20 2020 2020 2020 2020  venue:.         
-00021830: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-00021840: 6169 7420 7365 6c66 2e5f 636c 6965 6e74  ait self._client
-00021850: 2e73 656e 645f 7665 6e75 6528 0a20 2020  .send_venue(.   
-00021860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021870: 2063 6861 745f 6964 2c0a 2020 2020 2020   chat_id,.      
-00021880: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00021890: 7469 7475 6465 3d73 656c 662e 7665 6e75  titude=self.venu
-000218a0: 652e 6c6f 6361 7469 6f6e 2e6c 6174 6974  e.location.latit
+00021820: 6c6f 6361 7469 6f6e 3a0a 2020 2020 2020  location:.      
+00021830: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00021840: 2061 7761 6974 2073 656c 662e 5f63 6c69   await self._cli
+00021850: 656e 742e 7365 6e64 5f6c 6f63 6174 696f  ent.send_locatio
+00021860: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00021870: 2020 2020 2020 2063 6861 745f 6964 2c0a         chat_id,.
+00021880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021890: 2020 2020 6c61 7469 7475 6465 3d73 656c      latitude=sel
+000218a0: 662e 6c6f 6361 7469 6f6e 2e6c 6174 6974  f.location.latit
 000218b0: 7564 652c 0a20 2020 2020 2020 2020 2020  ude,.           
 000218c0: 2020 2020 2020 2020 206c 6f6e 6769 7475           longitu
-000218d0: 6465 3d73 656c 662e 7665 6e75 652e 6c6f  de=self.venue.lo
-000218e0: 6361 7469 6f6e 2e6c 6f6e 6769 7475 6465  cation.longitude
-000218f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021900: 2020 2020 2020 7469 746c 653d 7365 6c66        title=self
-00021910: 2e76 656e 7565 2e74 6974 6c65 2c0a 2020  .venue.title,.  
-00021920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021930: 2020 6164 6472 6573 733d 7365 6c66 2e76    address=self.v
-00021940: 656e 7565 2e61 6464 7265 7373 2c0a 2020  enue.address,.  
-00021950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021960: 2020 666f 7572 7371 7561 7265 5f69 643d    foursquare_id=
-00021970: 7365 6c66 2e76 656e 7565 2e66 6f75 7273  self.venue.fours
-00021980: 7175 6172 655f 6964 2c0a 2020 2020 2020  quare_id,.      
-00021990: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000219a0: 7572 7371 7561 7265 5f74 7970 653d 7365  ursquare_type=se
-000219b0: 6c66 2e76 656e 7565 2e66 6f75 7273 7175  lf.venue.foursqu
-000219c0: 6172 655f 7479 7065 2c0a 2020 2020 2020  are_type,.      
-000219d0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-000219e0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
-000219f0: 6f6e 3d64 6973 6162 6c65 5f6e 6f74 6966  on=disable_notif
-00021a00: 6963 6174 696f 6e2c 0a20 2020 2020 2020  ication,.       
-00021a10: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00021a20: 7361 6765 5f74 6872 6561 645f 6964 3d6d  sage_thread_id=m
-00021a30: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
-00021a40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021a50: 2020 2020 2020 7363 6865 6475 6c65 5f64        schedule_d
-00021a60: 6174 653d 7363 6865 6475 6c65 5f64 6174  ate=schedule_dat
-00021a70: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00021a80: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00021a90: 656c 6966 2073 656c 662e 706f 6c6c 3a0a  elif self.poll:.
-00021aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ab0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-00021ac0: 662e 5f63 6c69 656e 742e 7365 6e64 5f70  f._client.send_p
-00021ad0: 6f6c 6c28 0a20 2020 2020 2020 2020 2020  oll(.           
-00021ae0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-00021af0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021b00: 2020 2020 2020 7175 6573 7469 6f6e 3d73        question=s
-00021b10: 656c 662e 706f 6c6c 2e71 7565 7374 696f  elf.poll.questio
-00021b20: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00021b30: 2020 2020 2020 206f 7074 696f 6e73 3d5b         options=[
-00021b40: 6f70 742e 7465 7874 2066 6f72 206f 7074  opt.text for opt
-00021b50: 2069 6e20 7365 6c66 2e70 6f6c 6c2e 6f70   in self.poll.op
-00021b60: 7469 6f6e 735d 2c0a 2020 2020 2020 2020  tions],.        
-00021b70: 2020 2020 2020 2020 2020 2020 6469 7361              disa
-00021b80: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00021b90: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
-00021ba0: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
-00021bb0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00021bc0: 6765 5f74 6872 6561 645f 6964 3d6d 6573  ge_thread_id=mes
-00021bd0: 7361 6765 5f74 6872 6561 645f 6964 2c0a  sage_thread_id,.
+000218d0: 6465 3d73 656c 662e 6c6f 6361 7469 6f6e  de=self.location
+000218e0: 2e6c 6f6e 6769 7475 6465 2c0a 2020 2020  .longitude,.    
+000218f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021900: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00021910: 7469 6f6e 3d64 6973 6162 6c65 5f6e 6f74  tion=disable_not
+00021920: 6966 6963 6174 696f 6e2c 0a20 2020 2020  ification,.     
+00021930: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00021940: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+00021950: 3d6d 6573 7361 6765 5f74 6872 6561 645f  =message_thread_
+00021960: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00021970: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
+00021980: 5f64 6174 653d 7363 6865 6475 6c65 5f64  _date=schedule_d
+00021990: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
+000219a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+000219b0: 2020 656c 6966 2073 656c 662e 7665 6e75    elif self.venu
+000219c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000219d0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+000219e0: 7365 6c66 2e5f 636c 6965 6e74 2e73 656e  self._client.sen
+000219f0: 645f 7665 6e75 6528 0a20 2020 2020 2020  d_venue(.       
+00021a00: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00021a10: 745f 6964 2c0a 2020 2020 2020 2020 2020  t_id,.          
+00021a20: 2020 2020 2020 2020 2020 6c61 7469 7475            latitu
+00021a30: 6465 3d73 656c 662e 7665 6e75 652e 6c6f  de=self.venue.lo
+00021a40: 6361 7469 6f6e 2e6c 6174 6974 7564 652c  cation.latitude,
+00021a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021a60: 2020 2020 206c 6f6e 6769 7475 6465 3d73       longitude=s
+00021a70: 656c 662e 7665 6e75 652e 6c6f 6361 7469  elf.venue.locati
+00021a80: 6f6e 2e6c 6f6e 6769 7475 6465 2c0a 2020  on.longitude,.  
+00021a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021aa0: 2020 7469 746c 653d 7365 6c66 2e76 656e    title=self.ven
+00021ab0: 7565 2e74 6974 6c65 2c0a 2020 2020 2020  ue.title,.      
+00021ac0: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+00021ad0: 6472 6573 733d 7365 6c66 2e76 656e 7565  dress=self.venue
+00021ae0: 2e61 6464 7265 7373 2c0a 2020 2020 2020  .address,.      
+00021af0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00021b00: 7572 7371 7561 7265 5f69 643d 7365 6c66  ursquare_id=self
+00021b10: 2e76 656e 7565 2e66 6f75 7273 7175 6172  .venue.foursquar
+00021b20: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
+00021b30: 2020 2020 2020 2020 2020 666f 7572 7371            foursq
+00021b40: 7561 7265 5f74 7970 653d 7365 6c66 2e76  uare_type=self.v
+00021b50: 656e 7565 2e66 6f75 7273 7175 6172 655f  enue.foursquare_
+00021b60: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
+00021b70: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+00021b80: 655f 6e6f 7469 6669 6361 7469 6f6e 3d64  e_notification=d
+00021b90: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00021ba0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00021bb0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00021bc0: 5f74 6872 6561 645f 6964 3d6d 6573 7361  _thread_id=messa
+00021bd0: 6765 5f74 6872 6561 645f 6964 2c0a 2020  ge_thread_id,.  
 00021be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021bf0: 2020 2020 7363 6865 6475 6c65 5f64 6174      schedule_dat
-00021c00: 653d 7363 6865 6475 6c65 5f64 6174 650a  e=schedule_date.
-00021c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021c20: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00021c30: 6966 2073 656c 662e 6761 6d65 3a0a 2020  if self.game:.  
-00021c40: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00021c50: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-00021c60: 5f63 6c69 656e 742e 7365 6e64 5f67 616d  _client.send_gam
-00021c70: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00021c80: 2020 2020 2020 2063 6861 745f 6964 2c0a         chat_id,.
+00021bf0: 2020 7363 6865 6475 6c65 5f64 6174 653d    schedule_date=
+00021c00: 7363 6865 6475 6c65 5f64 6174 650a 2020  schedule_date.  
+00021c10: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00021c20: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00021c30: 2073 656c 662e 706f 6c6c 3a0a 2020 2020   self.poll:.    
+00021c40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00021c50: 726e 2061 7761 6974 2073 656c 662e 5f63  rn await self._c
+00021c60: 6c69 656e 742e 7365 6e64 5f70 6f6c 6c28  lient.send_poll(
+00021c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021c80: 2020 2020 2063 6861 745f 6964 2c0a 2020       chat_id,.  
 00021c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ca0: 2020 2020 6761 6d65 5f73 686f 7274 5f6e      game_short_n
-00021cb0: 616d 653d 7365 6c66 2e67 616d 652e 7368  ame=self.game.sh
-00021cc0: 6f72 745f 6e61 6d65 2c0a 2020 2020 2020  ort_name,.      
-00021cd0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00021ce0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
-00021cf0: 6f6e 3d64 6973 6162 6c65 5f6e 6f74 6966  on=disable_notif
-00021d00: 6963 6174 696f 6e2c 0a20 2020 2020 2020  ication,.       
-00021d10: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00021d20: 7361 6765 5f74 6872 6561 645f 6964 3d6d  sage_thread_id=m
-00021d30: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
-00021d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021d50: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
-00021d60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00021d70: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00021d80: 4572 726f 7228 2255 6e6b 6e6f 776e 206d  Error("Unknown m
-00021d90: 6564 6961 2074 7970 6522 290a 0a20 2020  edia type")..   
-00021da0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00021db0: 2e73 7469 636b 6572 206f 7220 7365 6c66  .sticker or self
-00021dc0: 2e76 6964 656f 5f6e 6f74 653a 2020 2320  .video_note:  # 
-00021dd0: 5374 6963 6b65 7220 616e 6420 5669 6465  Sticker and Vide
-00021de0: 6f4e 6f74 6520 7368 6f75 6c64 2068 6176  oNote should hav
-00021df0: 6520 6e6f 2063 6170 7469 6f6e 0a20 2020  e no caption.   
-00021e00: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00021e10: 7572 6e20 6177 6169 7420 7365 6e64 5f6d  urn await send_m
-00021e20: 6564 6961 280a 2020 2020 2020 2020 2020  edia(.          
-00021e30: 2020 2020 2020 2020 2020 6669 6c65 5f69            file_i
-00021e40: 643d 6669 6c65 5f69 642c 0a20 2020 2020  d=file_id,.     
-00021e50: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00021e60: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
-00021e70: 3d6d 6573 7361 6765 5f74 6872 6561 645f  =message_thread_
-00021e80: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
-00021e90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00021ea0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00021eb0: 2020 2020 2020 2069 6620 6361 7074 696f         if captio
-00021ec0: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-00021ed0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00021ee0: 6170 7469 6f6e 203d 2073 656c 662e 6361  aption = self.ca
-00021ef0: 7074 696f 6e20 6f72 2022 220a 2020 2020  ption or "".    
-00021f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021f10: 6361 7074 696f 6e5f 656e 7469 7469 6573  caption_entities
-00021f20: 203d 2073 656c 662e 6361 7074 696f 6e5f   = self.caption_
-00021f30: 656e 7469 7469 6573 0a0a 2020 2020 2020  entities..      
-00021f40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00021f50: 2061 7761 6974 2073 656e 645f 6d65 6469   await send_medi
-00021f60: 6128 0a20 2020 2020 2020 2020 2020 2020  a(.             
-00021f70: 2020 2020 2020 2066 696c 655f 6964 3d66         file_id=f
-00021f80: 696c 655f 6964 2c0a 2020 2020 2020 2020  ile_id,.        
-00021f90: 2020 2020 2020 2020 2020 2020 6361 7074              capt
-00021fa0: 696f 6e3d 6361 7074 696f 6e2c 0a20 2020  ion=caption,.   
-00021fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021fc0: 2070 6172 7365 5f6d 6f64 653d 7061 7273   parse_mode=pars
-00021fd0: 655f 6d6f 6465 2c0a 2020 2020 2020 2020  e_mode,.        
-00021fe0: 2020 2020 2020 2020 2020 2020 6361 7074              capt
-00021ff0: 696f 6e5f 656e 7469 7469 6573 3d63 6170  ion_entities=cap
-00022000: 7469 6f6e 5f65 6e74 6974 6965 732c 0a20  tion_entities,. 
-00022010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022020: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
-00022030: 645f 6964 3d6d 6573 7361 6765 5f74 6872  d_id=message_thr
-00022040: 6561 645f 6964 0a20 2020 2020 2020 2020  ead_id.         
-00022050: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00022060: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00022070: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00022080: 726f 7228 2243 616e 2774 2063 6f70 7920  ror("Can't copy 
-00022090: 7468 6973 206d 6573 7361 6765 2229 0a0a  this message")..
-000220a0: 2020 2020 6173 796e 6320 6465 6620 6465      async def de
-000220b0: 6c65 7465 2873 656c 662c 2072 6576 6f6b  lete(self, revok
-000220c0: 653a 2062 6f6f 6c20 3d20 5472 7565 293a  e: bool = True):
-000220d0: 0a20 2020 2020 2020 2022 2222 426f 756e  .        """Boun
-000220e0: 6420 6d65 7468 6f64 202a 6465 6c65 7465  d method *delete
-000220f0: 2a20 6f66 203a 6f62 6a3a 607e 7079 726f  * of :obj:`~pyro
-00022100: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
-00022110: 6765 602e 0a0a 2020 2020 2020 2020 5573  ge`...        Us
-00022120: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
-00022130: 666f 723a 0a0a 2020 2020 2020 2020 2e2e  for:..        ..
-00022140: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00022150: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-00022160: 2020 6177 6169 7420 636c 6965 6e74 2e64    await client.d
-00022170: 656c 6574 655f 6d65 7373 6167 6573 280a  elete_messages(.
-00022180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022190: 6368 6174 5f69 643d 6368 6174 5f69 642c  chat_id=chat_id,
-000221a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000221b0: 206d 6573 7361 6765 5f69 6473 3d6d 6573   message_ids=mes
-000221c0: 7361 6765 2e69 640a 2020 2020 2020 2020  sage.id.        
-000221d0: 2020 2020 290a 0a20 2020 2020 2020 2045      )..        E
-000221e0: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
-000221f0: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-00022200: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
-00022210: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00022220: 7420 6d65 7373 6167 652e 6465 6c65 7465  t message.delete
-00022230: 2829 0a0a 2020 2020 2020 2020 5061 7261  ()..        Para
-00022240: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
-00022250: 2020 2020 7265 766f 6b65 2028 6060 626f      revoke (``bo
-00022260: 6f6c 6060 2c20 2a6f 7074 696f 6e61 6c2a  ol``, *optional*
-00022270: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00022280: 2020 2044 656c 6574 6573 206d 6573 7361     Deletes messa
-00022290: 6765 7320 6f6e 2062 6f74 6820 7061 7274  ges on both part
-000222a0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-000222b0: 2020 2054 6869 7320 6973 206f 6e6c 7920     This is only 
-000222c0: 666f 7220 7072 6976 6174 6520 636c 6f75  for private clou
-000222d0: 6420 6368 6174 7320 616e 6420 6e6f 726d  d chats and norm
-000222e0: 616c 2067 726f 7570 732c 206d 6573 7361  al groups, messa
-000222f0: 6765 7320 6f6e 0a20 2020 2020 2020 2020  ges on.         
-00022300: 2020 2020 2020 2063 6861 6e6e 656c 7320         channels 
-00022310: 616e 6420 7375 7065 7267 726f 7570 7320  and supergroups 
-00022320: 6172 6520 616c 7761 7973 2072 6576 6f6b  are always revok
-00022330: 6564 2028 692e 652e 3a20 6465 6c65 7465  ed (i.e.: delete
-00022340: 6420 666f 7220 6576 6572 796f 6e65 292e  d for everyone).
-00022350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022360: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
-00022370: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-00022380: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00022390: 2054 7275 6520 6f6e 2073 7563 6365 7373   True on success
-000223a0: 2c20 4661 6c73 6520 6f74 6865 7277 6973  , False otherwis
-000223b0: 652e 0a0a 2020 2020 2020 2020 5261 6973  e...        Rais
-000223c0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-000223d0: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
-000223e0: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
-000223f0: 5250 4320 6572 726f 722e 0a20 2020 2020  RPC error..     
-00022400: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00022410: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-00022420: 2e5f 636c 6965 6e74 2e64 656c 6574 655f  ._client.delete_
-00022430: 6d65 7373 6167 6573 280a 2020 2020 2020  messages(.      
-00022440: 2020 2020 2020 6368 6174 5f69 643d 7365        chat_id=se
-00022450: 6c66 2e63 6861 742e 6964 2c0a 2020 2020  lf.chat.id,.    
-00022460: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
-00022470: 6964 733d 7365 6c66 2e69 642c 0a20 2020  ids=self.id,.   
-00022480: 2020 2020 2020 2020 2072 6576 6f6b 653d           revoke=
-00022490: 7265 766f 6b65 0a20 2020 2020 2020 2029  revoke.        )
-000224a0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-000224b0: 636c 6963 6b28 7365 6c66 2c20 783a 2055  click(self, x: U
-000224c0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 203d  nion[int, str] =
-000224d0: 2030 2c20 793a 2069 6e74 203d 204e 6f6e   0, y: int = Non
-000224e0: 652c 2071 756f 7465 3a20 626f 6f6c 203d  e, quote: bool =
-000224f0: 204e 6f6e 652c 2074 696d 656f 7574 3a20   None, timeout: 
-00022500: 696e 7420 3d20 3130 293a 0a20 2020 2020  int = 10):.     
-00022510: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
-00022520: 6f64 202a 636c 6963 6b2a 206f 6620 3a6f  od *click* of :o
-00022530: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
-00022540: 7065 732e 4d65 7373 6167 6560 2e0a 0a20  pes.Message`... 
-00022550: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
-00022560: 7368 6f72 7463 7574 2066 6f72 2063 6c69  shortcut for cli
-00022570: 636b 696e 6720 6120 6275 7474 6f6e 2061  cking a button a
-00022580: 7474 6163 6865 6420 746f 2074 6865 206d  ttached to the m
-00022590: 6573 7361 6765 2069 6e73 7465 6164 206f  essage instead o
-000225a0: 663a 0a0a 2020 2020 2020 2020 2d20 436c  f:..        - Cl
-000225b0: 6963 6b69 6e67 2069 6e6c 696e 6520 6275  icking inline bu
-000225c0: 7474 6f6e 733a 0a0a 2020 2020 2020 2020  ttons:..        
-000225d0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-000225e0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-000225f0: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
-00022600: 2e72 6571 7565 7374 5f63 616c 6c62 6163  .request_callbac
-00022610: 6b5f 616e 7377 6572 280a 2020 2020 2020  k_answer(.      
-00022620: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
-00022630: 643d 6d65 7373 6167 652e 6368 6174 2e69  d=message.chat.i
-00022640: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00022650: 2020 206d 6573 7361 6765 5f69 643d 6d65     message_id=me
-00022660: 7373 6167 652e 6964 2c0a 2020 2020 2020  ssage.id,.      
-00022670: 2020 2020 2020 2020 2020 6361 6c6c 6261            callba
-00022680: 636b 5f64 6174 613d 6d65 7373 6167 652e  ck_data=message.
-00022690: 7265 706c 795f 6d61 726b 7570 5b69 5d5b  reply_markup[i][
-000226a0: 6a5d 2e63 616c 6c62 6163 6b5f 6461 7461  j].callback_data
-000226b0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-000226c0: 2020 2020 2020 2020 2d20 436c 6963 6b69          - Clicki
-000226d0: 6e67 206e 6f72 6d61 6c20 6275 7474 6f6e  ng normal button
-000226e0: 733a 0a0a 2020 2020 2020 2020 2e2e 2063  s:..        .. c
-000226f0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-00022700: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-00022710: 6177 6169 7420 636c 6965 6e74 2e73 656e  await client.sen
-00022720: 645f 6d65 7373 6167 6528 0a20 2020 2020  d_message(.     
-00022730: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-00022740: 6964 3d6d 6573 7361 6765 2e63 6861 742e  id=message.chat.
-00022750: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00022760: 2020 2020 7465 7874 3d6d 6573 7361 6765      text=message
-00022770: 2e72 6570 6c79 5f6d 6172 6b75 705b 695d  .reply_markup[i]
-00022780: 5b6a 5d2e 7465 7874 0a20 2020 2020 2020  [j].text.       
-00022790: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-000227a0: 4578 616d 706c 653a 0a20 2020 2020 2020  Example:.       
-000227b0: 2020 2020 2054 6869 7320 6d65 7468 6f64       This method
-000227c0: 2063 616e 2062 6520 7573 6564 2069 6e20   can be used in 
-000227d0: 7468 7265 6520 6469 6666 6572 656e 7420  three different 
-000227e0: 7761 7973 3a0a 0a20 2020 2020 2020 2020  ways:..         
-000227f0: 2020 2031 2e20 2050 6173 7320 6f6e 6520     1.  Pass one 
-00022800: 696e 7465 6765 7220 6172 6775 6d65 6e74  integer argument
-00022810: 206f 6e6c 7920 2865 2e67 2e3a 2060 602e   only (e.g.: ``.
-00022820: 636c 6963 6b28 3229 6060 2c20 746f 2063  click(2)``, to c
-00022830: 6c69 636b 2061 2062 7574 746f 6e20 6174  lick a button at
-00022840: 2069 6e64 6578 2032 292e 0a20 2020 2020   index 2)..     
-00022850: 2020 2020 2020 2020 2020 2042 7574 746f             Butto
-00022860: 6e73 2061 7265 2063 6f75 6e74 6564 206c  ns are counted l
-00022870: 6566 7420 746f 2072 6967 6874 2c20 7374  eft to right, st
-00022880: 6172 7469 6e67 2066 726f 6d20 7468 6520  arting from the 
-00022890: 746f 702e 0a0a 2020 2020 2020 2020 2020  top...          
-000228a0: 2020 322e 2020 5061 7373 2074 776f 2069    2.  Pass two i
-000228b0: 6e74 6567 6572 2061 7267 756d 656e 7473  nteger arguments
-000228c0: 2028 652e 672e 3a20 6060 2e63 6c69 636b   (e.g.: ``.click
-000228d0: 2831 2c20 3029 6060 2c20 746f 2063 6c69  (1, 0)``, to cli
-000228e0: 636b 2061 2062 7574 746f 6e20 6174 2070  ck a button at p
-000228f0: 6f73 6974 696f 6e20 2831 2c20 3029 292e  osition (1, 0)).
-00022900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022910: 2054 6865 206f 7269 6769 6e20 2830 2c20   The origin (0, 
-00022920: 3029 2069 7320 746f 702d 6c65 6674 2e0a  0) is top-left..
-00022930: 0a20 2020 2020 2020 2020 2020 2033 2e20  .            3. 
-00022940: 2050 6173 7320 6f6e 6520 7374 7269 6e67   Pass one string
-00022950: 2061 7267 756d 656e 7420 6f6e 6c79 2028   argument only (
-00022960: 652e 672e 3a20 6060 2e63 6c69 636b 2822  e.g.: ``.click("
-00022970: 5365 7474 696e 6773 2229 6060 2c20 746f  Settings")``, to
-00022980: 2063 6c69 636b 2061 2062 7574 746f 6e20   click a button 
-00022990: 6279 2075 7369 6e67 2069 7473 206c 6162  by using its lab
-000229a0: 656c 292e 0a20 2020 2020 2020 2020 2020  el)..           
-000229b0: 2020 2020 204f 6e6c 7920 7468 6520 6669       Only the fi
-000229c0: 7273 7420 6d61 7463 6869 6e67 2062 7574  rst matching but
-000229d0: 746f 6e20 7769 6c6c 2062 6520 7072 6573  ton will be pres
-000229e0: 7365 642e 0a0a 2020 2020 2020 2020 5061  sed...        Pa
-000229f0: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-00022a00: 2020 2020 2020 7820 2860 6069 6e74 6060        x (``int``
-00022a10: 207c 2060 6073 7472 6060 293a 0a20 2020   | ``str``):.   
-00022a20: 2020 2020 2020 2020 2020 2020 2055 7365               Use
-00022a30: 6420 6173 2069 6e74 6567 6572 2069 6e64  d as integer ind
-00022a40: 6578 2c20 696e 7465 6765 7220 6162 7363  ex, integer absc
-00022a50: 6973 7361 2028 696e 2070 6169 7220 7769  issa (in pair wi
-00022a60: 7468 2079 2920 6f72 2061 7320 7374 7269  th y) or as stri
-00022a70: 6e67 206c 6162 656c 2e0a 2020 2020 2020  ng label..      
-00022a80: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00022a90: 7473 2074 6f20 3020 2866 6972 7374 2062  ts to 0 (first b
-00022aa0: 7574 746f 6e29 2e0a 0a20 2020 2020 2020  utton)...       
-00022ab0: 2020 2020 2079 2028 6060 696e 7460 602c       y (``int``,
-00022ac0: 202a 6f70 7469 6f6e 616c 2a29 3a0a 2020   *optional*):.  
-00022ad0: 2020 2020 2020 2020 2020 2020 2020 5573                Us
-00022ae0: 6564 2061 7320 6f72 6469 6e61 7465 206f  ed as ordinate o
-00022af0: 6e6c 7920 2869 6e20 7061 6972 2077 6974  nly (in pair wit
-00022b00: 6820 7829 2e0a 0a20 2020 2020 2020 2020  h x)...         
-00022b10: 2020 2071 756f 7465 2028 6060 626f 6f6c     quote (``bool
-00022b20: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
-00022b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022b40: 2055 7365 6675 6c20 666f 7220 6e6f 726d   Useful for norm
-00022b50: 616c 2062 7574 746f 6e73 206f 6e6c 792c  al buttons only,
-00022b60: 2077 6865 7265 2070 7265 7373 696e 6720   where pressing 
-00022b70: 6974 2077 696c 6c20 7265 7375 6c74 2069  it will result i
-00022b80: 6e20 6120 6e65 7720 6d65 7373 6167 6520  n a new message 
-00022b90: 7365 6e74 2e0a 2020 2020 2020 2020 2020  sent..          
-00022ba0: 2020 2020 2020 4966 2060 6054 7275 6560        If ``True`
-00022bb0: 602c 2074 6865 206d 6573 7361 6765 2077  `, the message w
-00022bc0: 696c 6c20 6265 2073 656e 7420 6173 2061  ill be sent as a
-00022bd0: 2072 6570 6c79 2074 6f20 7468 6973 206d   reply to this m
-00022be0: 6573 7361 6765 2e0a 2020 2020 2020 2020  essage..        
-00022bf0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00022c00: 2074 6f20 6060 5472 7565 6060 2069 6e20   to ``True`` in 
-00022c10: 6772 6f75 7020 6368 6174 7320 616e 6420  group chats and 
-00022c20: 6060 4661 6c73 6560 6020 696e 2070 7269  ``False`` in pri
-00022c30: 7661 7465 2063 6861 7473 2e0a 0a20 2020  vate chats...   
-00022c40: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-00022c50: 2028 6060 696e 7460 602c 202a 6f70 7469   (``int``, *opti
-00022c60: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
-00022c70: 2020 2020 2020 2020 5469 6d65 6f75 7420          Timeout 
-00022c80: 696e 2073 6563 6f6e 6473 2e0a 0a20 2020  in seconds...   
-00022c90: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00022ca0: 2020 2020 2020 2020 2020 2d20 2020 5468            -   Th
-00022cb0: 6520 7265 7375 6c74 206f 6620 3a6d 6574  e result of :met
-00022cc0: 683a 607e 7079 726f 6772 616d 2e43 6c69  h:`~pyrogram.Cli
-00022cd0: 656e 742e 7265 7175 6573 745f 6361 6c6c  ent.request_call
-00022ce0: 6261 636b 5f61 6e73 7765 7260 2069 6e20  back_answer` in 
-00022cf0: 6361 7365 206f 6620 696e 6c69 6e65 2063  case of inline c
-00022d00: 616c 6c62 6163 6b20 6275 7474 6f6e 2063  allback button c
-00022d10: 6c69 636b 732e 0a20 2020 2020 2020 2020  licks..         
-00022d20: 2020 202d 2020 2054 6865 2072 6573 756c     -   The resul
-00022d30: 7420 6f66 203a 6d65 7468 3a60 7e4d 6573  t of :meth:`~Mes
-00022d40: 7361 6765 2e72 6570 6c79 2829 6020 696e  sage.reply()` in
-00022d50: 2063 6173 6520 6f66 206e 6f72 6d61 6c20   case of normal 
-00022d60: 6275 7474 6f6e 2063 6c69 636b 732e 0a20  button clicks.. 
-00022d70: 2020 2020 2020 2020 2020 202d 2020 2041             -   A
-00022d80: 2073 7472 696e 6720 696e 2063 6173 6520   string in case 
-00022d90: 7468 6520 696e 6c69 6e65 2062 7574 746f  the inline butto
-00022da0: 6e20 6973 2061 2055 524c 2c20 6120 2a73  n is a URL, a *s
-00022db0: 7769 7463 685f 696e 6c69 6e65 5f71 7565  witch_inline_que
-00022dc0: 7279 2a20 6f72 2061 0a20 2020 2020 2020  ry* or a.       
-00022dd0: 2020 2020 2020 2020 202a 7377 6974 6368           *switch
-00022de0: 5f69 6e6c 696e 655f 7175 6572 795f 6375  _inline_query_cu
-00022df0: 7272 656e 745f 6368 6174 2a20 6275 7474  rrent_chat* butt
-00022e00: 6f6e 2e0a 0a20 2020 2020 2020 2052 6169  on...        Rai
-00022e10: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
-00022e20: 2052 5043 4572 726f 723a 2049 6e20 6361   RPCError: In ca
-00022e30: 7365 206f 6620 6120 5465 6c65 6772 616d  se of a Telegram
-00022e40: 2052 5043 2065 7272 6f72 2e0a 2020 2020   RPC error..    
-00022e50: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
-00022e60: 6f72 3a20 496e 2063 6173 6520 7468 6520  or: In case the 
-00022e70: 7072 6f76 6964 6564 2069 6e64 6578 206f  provided index o
-00022e80: 7220 706f 7369 7469 6f6e 2069 7320 6f75  r position is ou
-00022e90: 7420 6f66 2072 616e 6765 206f 7220 7468  t of range or th
-00022ea0: 6520 6275 7474 6f6e 206c 6162 656c 2077  e button label w
-00022eb0: 6173 206e 6f74 2066 6f75 6e64 2e0a 2020  as not found..  
-00022ec0: 2020 2020 2020 2020 2020 5469 6d65 6f75            Timeou
-00022ed0: 7445 7272 6f72 3a20 496e 2063 6173 652c  tError: In case,
-00022ee0: 2061 6674 6572 2063 6c69 636b 696e 6720   after clicking 
-00022ef0: 616e 2069 6e6c 696e 6520 6275 7474 6f6e  an inline button
-00022f00: 2c20 7468 6520 626f 7420 6661 696c 7320  , the bot fails 
-00022f10: 746f 2061 6e73 7765 7220 7769 7468 696e  to answer within
-00022f20: 2074 6865 2074 696d 656f 7574 2e0a 2020   the timeout..  
-00022f30: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00022f40: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00022f50: 2873 656c 662e 7265 706c 795f 6d61 726b  (self.reply_mark
-00022f60: 7570 2c20 7479 7065 732e 5265 706c 794b  up, types.ReplyK
-00022f70: 6579 626f 6172 644d 6172 6b75 7029 3a0a  eyboardMarkup):.
-00022f80: 2020 2020 2020 2020 2020 2020 6b65 7962              keyb
-00022f90: 6f61 7264 203d 2073 656c 662e 7265 706c  oard = self.repl
-00022fa0: 795f 6d61 726b 7570 2e6b 6579 626f 6172  y_markup.keyboar
-00022fb0: 640a 2020 2020 2020 2020 2020 2020 6973  d.            is
-00022fc0: 5f69 6e6c 696e 6520 3d20 4661 6c73 650a  _inline = False.
-00022fd0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-00022fe0: 6e73 7461 6e63 6528 7365 6c66 2e72 6570  nstance(self.rep
-00022ff0: 6c79 5f6d 6172 6b75 702c 2074 7970 6573  ly_markup, types
-00023000: 2e49 6e6c 696e 654b 6579 626f 6172 644d  .InlineKeyboardM
-00023010: 6172 6b75 7029 3a0a 2020 2020 2020 2020  arkup):.        
-00023020: 2020 2020 6b65 7962 6f61 7264 203d 2073      keyboard = s
-00023030: 656c 662e 7265 706c 795f 6d61 726b 7570  elf.reply_markup
-00023040: 2e69 6e6c 696e 655f 6b65 7962 6f61 7264  .inline_keyboard
-00023050: 0a20 2020 2020 2020 2020 2020 2069 735f  .            is_
-00023060: 696e 6c69 6e65 203d 2054 7275 650a 2020  inline = True.  
-00023070: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00023080: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00023090: 6c75 6545 7272 6f72 2822 5468 6520 6d65  lueError("The me
-000230a0: 7373 6167 6520 646f 6573 6e27 7420 636f  ssage doesn't co
-000230b0: 6e74 6169 6e20 616e 7920 6b65 7962 6f61  ntain any keyboa
-000230c0: 7264 2229 0a0a 2020 2020 2020 2020 6966  rd")..        if
-000230d0: 2069 7369 6e73 7461 6e63 6528 782c 2069   isinstance(x, i
-000230e0: 6e74 2920 616e 6420 7920 6973 204e 6f6e  nt) and y is Non
-000230f0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-00023100: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00023110: 2020 2020 6275 7474 6f6e 203d 205b 0a20      button = [. 
-00023120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023130: 2020 2062 7574 746f 6e0a 2020 2020 2020     button.      
-00023140: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00023150: 7220 726f 7720 696e 206b 6579 626f 6172  r row in keyboar
-00023160: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00023170: 2020 2020 2020 666f 7220 6275 7474 6f6e        for button
-00023180: 2069 6e20 726f 770a 2020 2020 2020 2020   in row.        
-00023190: 2020 2020 2020 2020 5d5b 785d 0a20 2020          ][x].   
-000231a0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-000231b0: 496e 6465 7845 7272 6f72 3a0a 2020 2020  IndexError:.    
-000231c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000231d0: 6520 5661 6c75 6545 7272 6f72 2866 2254  e ValueError(f"T
-000231e0: 6865 2062 7574 746f 6e20 6174 2069 6e64  he button at ind
-000231f0: 6578 207b 787d 2064 6f65 736e 2774 2065  ex {x} doesn't e
-00023200: 7869 7374 2229 0a20 2020 2020 2020 2065  xist").        e
-00023210: 6c69 6620 6973 696e 7374 616e 6365 2878  lif isinstance(x
-00023220: 2c20 696e 7429 2061 6e64 2069 7369 6e73  , int) and isins
-00023230: 7461 6e63 6528 792c 2069 6e74 293a 0a20  tance(y, int):. 
-00023240: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00023250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023260: 6275 7474 6f6e 203d 206b 6579 626f 6172  button = keyboar
-00023270: 645b 795d 5b78 5d0a 2020 2020 2020 2020  d[y][x].        
-00023280: 2020 2020 6578 6365 7074 2049 6e64 6578      except Index
-00023290: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-000232a0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-000232b0: 7565 4572 726f 7228 6622 5468 6520 6275  ueError(f"The bu
-000232c0: 7474 6f6e 2061 7420 706f 7369 7469 6f6e  tton at position
-000232d0: 2028 7b78 7d2c 207b 797d 2920 646f 6573   ({x}, {y}) does
-000232e0: 6e27 7420 6578 6973 7422 290a 2020 2020  n't exist").    
-000232f0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00023300: 6e63 6528 782c 2073 7472 2920 616e 6420  nce(x, str) and 
-00023310: 7920 6973 204e 6f6e 653a 0a20 2020 2020  y is None:.     
-00023320: 2020 2020 2020 206c 6162 656c 203d 2078         label = x
-00023330: 2e65 6e63 6f64 6528 2275 7466 2d31 3622  .encode("utf-16"
-00023340: 2c20 2273 7572 726f 6761 7465 7061 7373  , "surrogatepass
-00023350: 2229 2e64 6563 6f64 6528 2275 7466 2d31  ").decode("utf-1
-00023360: 3622 290a 0a20 2020 2020 2020 2020 2020  6")..           
-00023370: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00023380: 2020 2020 2020 6275 7474 6f6e 203d 205b        button = [
-00023390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000233a0: 2020 2020 2062 7574 746f 6e0a 2020 2020       button.    
-000233b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000233c0: 666f 7220 726f 7720 696e 206b 6579 626f  for row in keybo
-000233d0: 6172 640a 2020 2020 2020 2020 2020 2020  ard.            
-000233e0: 2020 2020 2020 2020 666f 7220 6275 7474          for butt
-000233f0: 6f6e 2069 6e20 726f 770a 2020 2020 2020  on in row.      
-00023400: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00023410: 206c 6162 656c 203d 3d20 6275 7474 6f6e   label == button
-00023420: 2e74 6578 740a 2020 2020 2020 2020 2020  .text.          
-00023430: 2020 2020 2020 5d5b 305d 0a20 2020 2020        ][0].     
-00023440: 2020 2020 2020 2065 7863 6570 7420 496e         except In
-00023450: 6465 7845 7272 6f72 3a0a 2020 2020 2020  dexError:.      
-00023460: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00023470: 5661 6c75 6545 7272 6f72 2866 2254 6865  ValueError(f"The
-00023480: 2062 7574 746f 6e20 7769 7468 206c 6162   button with lab
-00023490: 656c 2027 7b78 7d27 2064 6f65 736e 2774  el '{x}' doesn't
-000234a0: 2065 7869 7374 7322 290a 2020 2020 2020   exists").      
-000234b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000234c0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-000234d0: 7272 6f72 2822 496e 7661 6c69 6420 6172  rror("Invalid ar
-000234e0: 6775 6d65 6e74 7322 290a 0a20 2020 2020  guments")..     
-000234f0: 2020 2069 6620 6973 5f69 6e6c 696e 653a     if is_inline:
-00023500: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00023510: 6275 7474 6f6e 2e63 616c 6c62 6163 6b5f  button.callback_
-00023520: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-00023530: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-00023540: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-00023550: 7265 7175 6573 745f 6361 6c6c 6261 636b  request_callback
-00023560: 5f61 6e73 7765 7228 0a20 2020 2020 2020  _answer(.       
-00023570: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00023580: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
-00023590: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-000235a0: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-000235b0: 643d 7365 6c66 2e69 642c 0a20 2020 2020  d=self.id,.     
-000235c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000235d0: 616c 6c62 6163 6b5f 6461 7461 3d62 7574  allback_data=but
-000235e0: 746f 6e2e 6361 6c6c 6261 636b 5f64 6174  ton.callback_dat
-000235f0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-00023600: 2020 2020 2020 2074 696d 656f 7574 3d74         timeout=t
-00023610: 696d 656f 7574 0a20 2020 2020 2020 2020  imeout.         
-00023620: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00023630: 2020 2020 2065 6c69 6620 6275 7474 6f6e       elif button
-00023640: 2e75 726c 3a0a 2020 2020 2020 2020 2020  .url:.          
-00023650: 2020 2020 2020 7265 7475 726e 2062 7574        return but
-00023660: 746f 6e2e 7572 6c0a 2020 2020 2020 2020  ton.url.        
-00023670: 2020 2020 656c 6966 2062 7574 746f 6e2e      elif button.
-00023680: 7377 6974 6368 5f69 6e6c 696e 655f 7175  switch_inline_qu
-00023690: 6572 793a 0a20 2020 2020 2020 2020 2020  ery:.           
-000236a0: 2020 2020 2072 6574 7572 6e20 6275 7474       return butt
-000236b0: 6f6e 2e73 7769 7463 685f 696e 6c69 6e65  on.switch_inline
-000236c0: 5f71 7565 7279 0a20 2020 2020 2020 2020  _query.         
-000236d0: 2020 2065 6c69 6620 6275 7474 6f6e 2e73     elif button.s
-000236e0: 7769 7463 685f 696e 6c69 6e65 5f71 7565  witch_inline_que
-000236f0: 7279 5f63 7572 7265 6e74 5f63 6861 743a  ry_current_chat:
-00023700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023710: 2072 6574 7572 6e20 6275 7474 6f6e 2e73   return button.s
-00023720: 7769 7463 685f 696e 6c69 6e65 5f71 7565  witch_inline_que
-00023730: 7279 5f63 7572 7265 6e74 5f63 6861 740a  ry_current_chat.
-00023740: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00023750: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00023760: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00023770: 6f72 2822 5468 6973 2062 7574 746f 6e20  or("This button 
-00023780: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
-00023790: 2079 6574 2229 0a20 2020 2020 2020 2065   yet").        e
-000237a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000237b0: 2061 7761 6974 2073 656c 662e 7265 706c   await self.repl
-000237c0: 7928 6275 7474 6f6e 2c20 7175 6f74 653d  y(button, quote=
-000237d0: 7175 6f74 6529 0a0a 2020 2020 6173 796e  quote)..    asyn
-000237e0: 6320 6465 6620 7265 6163 7428 7365 6c66  c def react(self
-000237f0: 2c20 656d 6f6a 693a 2073 7472 203d 2022  , emoji: str = "
-00023800: 222c 2062 6967 3a20 626f 6f6c 203d 2046  ", big: bool = F
-00023810: 616c 7365 2920 2d3e 2062 6f6f 6c3a 0a20  alse) -> bool:. 
-00023820: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
-00023830: 6d65 7468 6f64 202a 7265 6163 742a 206f  method *react* o
-00023840: 6620 3a6f 626a 3a60 7e70 7972 6f67 7261  f :obj:`~pyrogra
-00023850: 6d2e 7479 7065 732e 4d65 7373 6167 6560  m.types.Message`
-00023860: 2e0a 0a20 2020 2020 2020 2055 7365 2061  ...        Use a
-00023870: 7320 6120 7368 6f72 7463 7574 2066 6f72  s a shortcut for
-00023880: 3a0a 0a20 2020 2020 2020 202e 2e20 636f  :..        .. co
-00023890: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
-000238a0: 6e0a 0a20 2020 2020 2020 2020 2020 2061  n..            a
-000238b0: 7761 6974 2063 6c69 656e 742e 7365 6e64  wait client.send
-000238c0: 5f72 6561 6374 696f 6e28 0a20 2020 2020  _reaction(.     
-000238d0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-000238e0: 6964 3d63 6861 745f 6964 2c0a 2020 2020  id=chat_id,.    
-000238f0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00023900: 6167 655f 6964 3d6d 6573 7361 6765 2e69  age_id=message.i
-00023910: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00023920: 2020 2065 6d6f 6a69 3d22 f09f 94a5 220a     emoji="....".
-00023930: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00023940: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-00023950: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
-00023960: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-00023970: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-00023980: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-00023990: 652e 7265 6163 7428 656d 6f6a 693d 22f0  e.react(emoji=".
-000239a0: 9f94 a522 290a 0a20 2020 2020 2020 2050  ...")..        P
-000239b0: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
-000239c0: 2020 2020 2020 2065 6d6f 6a69 2028 6060         emoji (``
-000239d0: 7374 7260 602c 202a 6f70 7469 6f6e 616c  str``, *optional
-000239e0: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-000239f0: 2020 2020 5265 6163 7469 6f6e 2065 6d6f      Reaction emo
-00023a00: 6a69 2e0a 2020 2020 2020 2020 2020 2020  ji..            
-00023a10: 2020 2020 5061 7373 2022 2220 6173 2065      Pass "" as e
-00023a20: 6d6f 6a69 2028 6465 6661 756c 7429 2074  moji (default) t
-00023a30: 6f20 7265 7472 6163 7420 7468 6520 7265  o retract the re
-00023a40: 6163 7469 6f6e 2e0a 2020 2020 2020 2020  action..        
-00023a50: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00023a60: 2020 6269 6720 2860 6062 6f6f 6c60 602c    big (``bool``,
-00023a70: 202a 6f70 7469 6f6e 616c 2a29 3a0a 2020   *optional*):.  
-00023a80: 2020 2020 2020 2020 2020 2020 2020 5061                Pa
-00023a90: 7373 2054 7275 6520 746f 2073 686f 7720  ss True to show 
-00023aa0: 6120 6269 6767 6572 2061 6e64 206c 6f6e  a bigger and lon
-00023ab0: 6765 7220 7265 6163 7469 6f6e 2e0a 2020  ger reaction..  
-00023ac0: 2020 2020 2020 2020 2020 2020 2020 4465                De
-00023ad0: 6661 756c 7473 2074 6f20 4661 6c73 652e  faults to False.
-00023ae0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00023af0: 733a 0a20 2020 2020 2020 2020 2020 2060  s:.            `
-00023b00: 6062 6f6f 6c60 603a 204f 6e20 7375 6363  `bool``: On succ
-00023b10: 6573 732c 2054 7275 6520 6973 2072 6574  ess, True is ret
-00023b20: 7572 6e65 642e 0a0a 2020 2020 2020 2020  urned...        
-00023b30: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00023b40: 2020 2020 5250 4345 7272 6f72 3a20 496e      RPCError: In
-00023b50: 2063 6173 6520 6f66 2061 2054 656c 6567   case of a Teleg
-00023b60: 7261 6d20 5250 4320 6572 726f 722e 0a20  ram RPC error.. 
-00023b70: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00023b80: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00023b90: 2073 656c 662e 5f63 6c69 656e 742e 7365   self._client.se
-00023ba0: 6e64 5f72 6561 6374 696f 6e28 0a20 2020  nd_reaction(.   
-00023bb0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-00023bc0: 3d73 656c 662e 6368 6174 2e69 642c 0a20  =self.chat.id,. 
-00023bd0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00023be0: 6765 5f69 643d 7365 6c66 2e69 642c 0a20  ge_id=self.id,. 
-00023bf0: 2020 2020 2020 2020 2020 2065 6d6f 6a69             emoji
-00023c00: 3d65 6d6f 6a69 2c0a 2020 2020 2020 2020  =emoji,.        
-00023c10: 2020 2020 6269 673d 6269 670a 2020 2020      big=big.    
-00023c20: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
-00023c30: 2064 6566 2072 6574 7261 6374 5f76 6f74   def retract_vot
-00023c40: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
-00023c50: 0a20 2020 2029 202d 3e20 2274 7970 6573  .    ) -> "types
-00023c60: 2e50 6f6c 6c22 3a0a 2020 2020 2020 2020  .Poll":.        
-00023c70: 2222 2242 6f75 6e64 206d 6574 686f 6420  """Bound method 
-00023c80: 2a72 6574 7261 6374 5f76 6f74 652a 206f  *retract_vote* o
-00023c90: 6620 3a6f 626a 3a60 7e70 7972 6f67 7261  f :obj:`~pyrogra
-00023ca0: 6d2e 7479 7065 732e 4d65 7373 6167 6560  m.types.Message`
-00023cb0: 2e0a 0a20 2020 2020 2020 2055 7365 2061  ...        Use a
-00023cc0: 7320 6120 7368 6f72 7463 7574 2066 6f72  s a shortcut for
-00023cd0: 3a0a 0a20 2020 2020 2020 202e 2e20 636f  :..        .. co
-00023ce0: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
-00023cf0: 6e0a 0a20 2020 2020 2020 2020 2020 2063  n..            c
-00023d00: 6c69 656e 742e 7265 7472 6163 745f 766f  lient.retract_vo
-00023d10: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
-00023d20: 2020 2020 6368 6174 5f69 643d 6d65 7373      chat_id=mess
-00023d30: 6167 652e 6368 6174 2e69 642c 0a20 2020  age.chat.id,.   
-00023d40: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00023d50: 7361 6765 5f69 643d 6d65 7373 6167 655f  sage_id=message_
-00023d60: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00023d70: 290a 0a20 2020 2020 2020 2045 7861 6d70  )..        Examp
-00023d80: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00023d90: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-00023da0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-00023db0: 2020 2020 2020 2020 6d65 7373 6167 652e          message.
-00023dc0: 7265 7472 6163 745f 766f 7465 2829 0a0a  retract_vote()..
-00023dd0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00023de0: 0a20 2020 2020 2020 2020 2020 203a 6f62  .            :ob
-00023df0: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
-00023e00: 6573 2e50 6f6c 6c60 3a20 4f6e 2073 7563  es.Poll`: On suc
-00023e10: 6365 7373 2c20 7468 6520 706f 6c6c 2077  cess, the poll w
-00023e20: 6974 6820 7468 6520 7265 7472 6163 7465  ith the retracte
-00023e30: 6420 766f 7465 2069 7320 7265 7475 726e  d vote is return
-00023e40: 6564 2e0a 0a20 2020 2020 2020 2052 6169  ed...        Rai
-00023e50: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
-00023e60: 2052 5043 4572 726f 723a 2049 6e20 6361   RPCError: In ca
-00023e70: 7365 206f 6620 6120 5465 6c65 6772 616d  se of a Telegram
-00023e80: 2052 5043 2065 7272 6f72 2e0a 2020 2020   RPC error..    
-00023e90: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00023ea0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-00023eb0: 6c66 2e5f 636c 6965 6e74 2e72 6574 7261  lf._client.retra
-00023ec0: 6374 5f76 6f74 6528 0a20 2020 2020 2020  ct_vote(.       
-00023ed0: 2020 2020 2063 6861 745f 6964 3d73 656c       chat_id=sel
-00023ee0: 662e 6368 6174 2e69 642c 0a20 2020 2020  f.chat.id,.     
-00023ef0: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-00023f00: 643d 7365 6c66 2e69 640a 2020 2020 2020  d=self.id.      
-00023f10: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
-00023f20: 6566 2064 6f77 6e6c 6f61 6428 0a20 2020  ef download(.   
-00023f30: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00023f40: 2020 2066 696c 655f 6e61 6d65 3a20 7374     file_name: st
-00023f50: 7220 3d20 2222 2c0a 2020 2020 2020 2020  r = "",.        
-00023f60: 696e 5f6d 656d 6f72 793a 2062 6f6f 6c20  in_memory: bool 
-00023f70: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
-00023f80: 2062 6c6f 636b 3a20 626f 6f6c 203d 2054   block: bool = T
-00023f90: 7275 652c 0a20 2020 2020 2020 2070 726f  rue,.        pro
-00023fa0: 6772 6573 733a 2043 616c 6c61 626c 6520  gress: Callable 
-00023fb0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00023fc0: 7072 6f67 7265 7373 5f61 7267 733a 2074  progress_args: t
-00023fd0: 7570 6c65 203d 2028 290a 2020 2020 2920  uple = ().    ) 
-00023fe0: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-00023ff0: 2222 2242 6f75 6e64 206d 6574 686f 6420  """Bound method 
-00024000: 2a64 6f77 6e6c 6f61 642a 206f 6620 3a6f  *download* of :o
-00024010: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
-00024020: 7065 732e 4d65 7373 6167 6560 2e0a 0a20  pes.Message`... 
-00024030: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
-00024040: 7368 6f72 7463 7574 2066 6f72 3a0a 0a20  shortcut for:.. 
-00024050: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
-00024060: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
-00024070: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00024080: 2063 6c69 656e 742e 646f 776e 6c6f 6164   client.download
-00024090: 5f6d 6564 6961 286d 6573 7361 6765 290a  _media(message).
-000240a0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-000240b0: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-000240c0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-000240d0: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-000240e0: 2020 2020 2020 6177 6169 7420 6d65 7373        await mess
-000240f0: 6167 652e 646f 776e 6c6f 6164 2829 0a0a  age.download()..
-00024100: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00024110: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-00024120: 6669 6c65 5f6e 616d 6520 2860 6073 7472  file_name (``str
-00024130: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
-00024140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024150: 2041 2063 7573 746f 6d20 2a66 696c 655f   A custom *file_
-00024160: 6e61 6d65 2a20 746f 2062 6520 7573 6564  name* to be used
-00024170: 2069 6e73 7465 6164 206f 6620 7468 6520   instead of the 
-00024180: 6f6e 6520 7072 6f76 6964 6564 2062 7920  one provided by 
-00024190: 5465 6c65 6772 616d 2e0a 2020 2020 2020  Telegram..      
-000241a0: 2020 2020 2020 2020 2020 4279 2064 6566            By def
-000241b0: 6175 6c74 2c20 616c 6c20 6669 6c65 7320  ault, all files 
-000241c0: 6172 6520 646f 776e 6c6f 6164 6564 2069  are downloaded i
-000241d0: 6e20 7468 6520 2a64 6f77 6e6c 6f61 6473  n the *downloads
-000241e0: 2a20 666f 6c64 6572 2069 6e20 796f 7572  * folder in your
-000241f0: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
-00024200: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
-00024210: 2020 2020 596f 7520 6361 6e20 616c 736f      You can also
-00024220: 2073 7065 6369 6679 2061 2070 6174 6820   specify a path 
-00024230: 666f 7220 646f 776e 6c6f 6164 696e 6720  for downloading 
-00024240: 6669 6c65 7320 696e 2061 2063 7573 746f  files in a custo
-00024250: 6d20 6c6f 6361 7469 6f6e 3a20 7061 7468  m location: path
-00024260: 7320 7468 6174 2065 6e64 2077 6974 6820  s that end with 
-00024270: 222f 220a 2020 2020 2020 2020 2020 2020  "/".            
-00024280: 2020 2020 6172 6520 636f 6e73 6964 6572      are consider
-00024290: 6564 2064 6972 6563 746f 7269 6573 2e20  ed directories. 
-000242a0: 416c 6c20 6e6f 6e2d 6578 6973 7465 6e74  All non-existent
-000242b0: 2066 6f6c 6465 7273 2077 696c 6c20 6265   folders will be
-000242c0: 2063 7265 6174 6564 2061 7574 6f6d 6174   created automat
-000242d0: 6963 616c 6c79 2e0a 0a20 2020 2020 2020  ically...       
-000242e0: 2020 2020 2069 6e5f 6d65 6d6f 7279 2028       in_memory (
-000242f0: 6060 626f 6f6c 6060 2c20 2a6f 7074 696f  ``bool``, *optio
-00024300: 6e61 6c2a 293a 0a20 2020 2020 2020 2020  nal*):.         
-00024310: 2020 2020 2020 2050 6173 7320 5472 7565         Pass True
-00024320: 2074 6f20 646f 776e 6c6f 6164 2074 6865   to download the
-00024330: 206d 6564 6961 2069 6e2d 6d65 6d6f 7279   media in-memory
-00024340: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00024350: 2020 4120 6269 6e61 7279 2066 696c 652d    A binary file-
-00024360: 6c69 6b65 206f 626a 6563 7420 7769 7468  like object with
-00024370: 2069 7473 2061 7474 7269 6275 7465 2022   its attribute "
-00024380: 2e6e 616d 6522 2073 6574 2077 696c 6c20  .name" set will 
-00024390: 6265 2072 6574 7572 6e65 642e 0a20 2020  be returned..   
-000243a0: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-000243b0: 6175 6c74 7320 746f 2046 616c 7365 2e0a  aults to False..
-000243c0: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
-000243d0: 636b 2028 6060 626f 6f6c 6060 2c20 2a6f  ck (``bool``, *o
-000243e0: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-000243f0: 2020 2020 2020 2020 2020 2042 6c6f 636b             Block
-00024400: 7320 7468 6520 636f 6465 2065 7865 6375  s the code execu
-00024410: 7469 6f6e 2075 6e74 696c 2074 6865 2066  tion until the f
-00024420: 696c 6520 6861 7320 6265 656e 2064 6f77  ile has been dow
-00024430: 6e6c 6f61 6465 642e 0a20 2020 2020 2020  nloaded..       
-00024440: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00024450: 7320 746f 2054 7275 652e 0a0a 2020 2020  s to True...    
-00024460: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
-00024470: 2028 6060 4361 6c6c 6162 6c65 6060 2c20   (``Callable``, 
-00024480: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
-00024490: 2020 2020 2020 2020 2020 2020 2050 6173               Pas
-000244a0: 7320 6120 6361 6c6c 6261 636b 2066 756e  s a callback fun
-000244b0: 6374 696f 6e20 746f 2076 6965 7720 7468  ction to view th
-000244c0: 6520 6669 6c65 2074 7261 6e73 6d69 7373  e file transmiss
-000244d0: 696f 6e20 7072 6f67 7265 7373 2e0a 2020  ion progress..  
-000244e0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
-000244f0: 6520 6675 6e63 7469 6f6e 206d 7573 7420  e function must 
-00024500: 7461 6b65 202a 2863 7572 7265 6e74 2c20  take *(current, 
-00024510: 746f 7461 6c29 2a20 6173 2070 6f73 6974  total)* as posit
-00024520: 696f 6e61 6c20 6172 6775 6d65 6e74 7320  ional arguments 
-00024530: 286c 6f6f 6b20 6174 204f 7468 6572 2050  (look at Other P
-00024540: 6172 616d 6574 6572 7320 6265 6c6f 7720  arameters below 
-00024550: 666f 7220 610a 2020 2020 2020 2020 2020  for a.          
-00024560: 2020 2020 2020 6465 7461 696c 6564 2064        detailed d
-00024570: 6573 6372 6970 7469 6f6e 2920 616e 6420  escription) and 
-00024580: 7769 6c6c 2062 6520 6361 6c6c 6564 2062  will be called b
-00024590: 6163 6b20 6561 6368 2074 696d 6520 6120  ack each time a 
-000245a0: 6e65 7720 6669 6c65 2063 6875 6e6b 2068  new file chunk h
-000245b0: 6173 2062 6565 6e20 7375 6363 6573 7366  as been successf
-000245c0: 756c 6c79 0a20 2020 2020 2020 2020 2020  ully.           
-000245d0: 2020 2020 2074 7261 6e73 6d69 7474 6564       transmitted
-000245e0: 2e0a 0a20 2020 2020 2020 2020 2020 2070  ...            p
-000245f0: 726f 6772 6573 735f 6172 6773 2028 6060  rogress_args (``
-00024600: 7475 706c 6560 602c 202a 6f70 7469 6f6e  tuple``, *option
-00024610: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
-00024620: 2020 2020 2020 4578 7472 6120 6375 7374        Extra cust
-00024630: 6f6d 2061 7267 756d 656e 7473 2066 6f72  om arguments for
-00024640: 2074 6865 2070 726f 6772 6573 7320 6361   the progress ca
-00024650: 6c6c 6261 636b 2066 756e 6374 696f 6e2e  llback function.
-00024660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024670: 2059 6f75 2063 616e 2070 6173 7320 616e   You can pass an
-00024680: 7974 6869 6e67 2079 6f75 206e 6565 6420  ything you need 
-00024690: 746f 2062 6520 6176 6169 6c61 626c 6520  to be available 
-000246a0: 696e 2074 6865 2070 726f 6772 6573 7320  in the progress 
-000246b0: 6361 6c6c 6261 636b 2073 636f 7065 3b20  callback scope; 
-000246c0: 666f 7220 6578 616d 706c 652c 2061 204d  for example, a M
-000246d0: 6573 7361 6765 0a20 2020 2020 2020 2020  essage.         
-000246e0: 2020 2020 2020 206f 626a 6563 7420 6f72         object or
-000246f0: 2061 2043 6c69 656e 7420 696e 7374 616e   a Client instan
-00024700: 6365 2069 6e20 6f72 6465 7220 746f 2065  ce in order to e
-00024710: 6469 7420 7468 6520 6d65 7373 6167 6520  dit the message 
-00024720: 7769 7468 2074 6865 2075 7064 6174 6564  with the updated
-00024730: 2070 726f 6772 6573 7320 7374 6174 7573   progress status
-00024740: 2e0a 0a20 2020 2020 2020 204f 7468 6572  ...        Other
-00024750: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
-00024760: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00024770: 2028 6060 696e 7460 6029 3a0a 2020 2020   (``int``):.    
-00024780: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00024790: 616d 6f75 6e74 206f 6620 6279 7465 7320  amount of bytes 
-000247a0: 7472 616e 736d 6974 7465 6420 736f 2066  transmitted so f
-000247b0: 6172 2e0a 0a20 2020 2020 2020 2020 2020  ar...           
-000247c0: 2074 6f74 616c 2028 6060 696e 7460 6029   total (``int``)
-000247d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000247e0: 2020 5468 6520 746f 7461 6c20 7369 7a65    The total size
-000247f0: 206f 6620 7468 6520 6669 6c65 2e0a 0a20   of the file... 
-00024800: 2020 2020 2020 2020 2020 202a 6172 6773             *args
-00024810: 2028 6060 7475 706c 6560 602c 202a 6f70   (``tuple``, *op
-00024820: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
-00024830: 2020 2020 2020 2020 2020 4578 7472 6120            Extra 
-00024840: 6375 7374 6f6d 2061 7267 756d 656e 7473  custom arguments
-00024850: 2061 7320 6465 6669 6e65 6420 696e 2074   as defined in t
-00024860: 6865 2060 6070 726f 6772 6573 735f 6172  he ``progress_ar
-00024870: 6773 6060 2070 6172 616d 6574 6572 2e0a  gs`` parameter..
-00024880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024890: 596f 7520 6361 6e20 6569 7468 6572 206b  You can either k
-000248a0: 6565 7020 6060 2a61 7267 7360 6020 6f72  eep ``*args`` or
-000248b0: 2061 6464 2065 7665 7279 2073 696e 676c   add every singl
-000248c0: 6520 6578 7472 6120 6172 6775 6d65 6e74  e extra argument
-000248d0: 2069 6e20 796f 7572 2066 756e 6374 696f   in your functio
-000248e0: 6e20 7369 676e 6174 7572 652e 0a0a 2020  n signature...  
-000248f0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00024900: 2020 2020 2020 2020 2020 204f 6e20 7375             On su
-00024910: 6363 6573 732c 2074 6865 2061 6273 6f6c  ccess, the absol
-00024920: 7574 6520 7061 7468 206f 6620 7468 6520  ute path of the 
-00024930: 646f 776e 6c6f 6164 6564 2066 696c 6520  downloaded file 
-00024940: 6173 2073 7472 696e 6720 6973 2072 6574  as string is ret
-00024950: 7572 6e65 642c 204e 6f6e 6520 6f74 6865  urned, None othe
-00024960: 7277 6973 652e 0a0a 2020 2020 2020 2020  rwise...        
-00024970: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00024980: 2020 2020 5250 4345 7272 6f72 3a20 496e      RPCError: In
-00024990: 2063 6173 6520 6f66 2061 2054 656c 6567   case of a Teleg
-000249a0: 7261 6d20 5250 4320 6572 726f 722e 0a20  ram RPC error.. 
-000249b0: 2020 2020 2020 2020 2020 2060 6056 616c             ``Val
-000249c0: 7565 4572 726f 7260 603a 2049 6620 7468  ueError``: If th
-000249d0: 6520 6d65 7373 6167 6520 646f 6573 6e27  e message doesn'
-000249e0: 7420 636f 6e74 6169 6e20 616e 7920 646f  t contain any do
-000249f0: 776e 6c6f 6164 6162 6c65 206d 6564 6961  wnloadable media
-00024a00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00024a10: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-00024a20: 7420 7365 6c66 2e5f 636c 6965 6e74 2e64  t self._client.d
-00024a30: 6f77 6e6c 6f61 645f 6d65 6469 6128 0a20  ownload_media(. 
-00024a40: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00024a50: 6765 3d73 656c 662c 0a20 2020 2020 2020  ge=self,.       
-00024a60: 2020 2020 2066 696c 655f 6e61 6d65 3d66       file_name=f
-00024a70: 696c 655f 6e61 6d65 2c0a 2020 2020 2020  ile_name,.      
-00024a80: 2020 2020 2020 696e 5f6d 656d 6f72 793d        in_memory=
-00024a90: 696e 5f6d 656d 6f72 792c 0a20 2020 2020  in_memory,.     
-00024aa0: 2020 2020 2020 2062 6c6f 636b 3d62 6c6f         block=blo
-00024ab0: 636b 2c0a 2020 2020 2020 2020 2020 2020  ck,.            
-00024ac0: 7072 6f67 7265 7373 3d70 726f 6772 6573  progress=progres
-00024ad0: 732c 0a20 2020 2020 2020 2020 2020 2070  s,.            p
-00024ae0: 726f 6772 6573 735f 6172 6773 3d70 726f  rogress_args=pro
-00024af0: 6772 6573 735f 6172 6773 2c0a 2020 2020  gress_args,.    
-00024b00: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
-00024b10: 2064 6566 2076 6f74 6528 0a20 2020 2020   def vote(.     
-00024b20: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00024b30: 206f 7074 696f 6e3a 2069 6e74 2c0a 2020   option: int,.  
-00024b40: 2020 2920 2d3e 2022 7479 7065 732e 506f    ) -> "types.Po
-00024b50: 6c6c 223a 0a20 2020 2020 2020 2022 2222  ll":.        """
-00024b60: 426f 756e 6420 6d65 7468 6f64 202a 766f  Bound method *vo
-00024b70: 7465 2a20 6f66 203a 6f62 6a3a 607e 7079  te* of :obj:`~py
-00024b80: 726f 6772 616d 2e74 7970 6573 2e4d 6573  rogram.types.Mes
-00024b90: 7361 6765 602e 0a0a 2020 2020 2020 2020  sage`...        
-00024ba0: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
-00024bb0: 7420 666f 723a 0a0a 2020 2020 2020 2020  t for:..        
-00024bc0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-00024bd0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-00024be0: 2020 2020 636c 6965 6e74 2e76 6f74 655f      client.vote_
-00024bf0: 706f 6c6c 280a 2020 2020 2020 2020 2020  poll(.          
-00024c00: 2020 2020 2020 6368 6174 5f69 643d 6d65        chat_id=me
-00024c10: 7373 6167 652e 6368 6174 2e69 642c 0a20  ssage.chat.id,. 
-00024c20: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00024c30: 6573 7361 6765 5f69 643d 6d65 7373 6167  essage_id=messag
-00024c40: 652e 6964 2c0a 2020 2020 2020 2020 2020  e.id,.          
-00024c50: 2020 2020 2020 6f70 7469 6f6e 3d31 0a20        option=1. 
-00024c60: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00024c70: 2020 2020 2020 4578 616d 706c 653a 0a20        Example:. 
-00024c80: 2020 2020 2020 2020 2020 202e 2e20 636f             .. co
-00024c90: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
-00024ca0: 6e0a 0a20 2020 2020 2020 2020 2020 2020  n..             
-00024cb0: 2020 206d 6573 7361 6765 2e76 6f74 6528     message.vote(
-00024cc0: 3629 0a0a 2020 2020 2020 2020 5061 7261  6)..        Para
-00024cd0: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
-00024ce0: 2020 2020 6f70 7469 6f6e 2028 6060 696e      option (``in
-00024cf0: 7460 6029 3a0a 2020 2020 2020 2020 2020  t``):.          
-00024d00: 2020 2020 2020 496e 6465 7820 6f66 2074        Index of t
-00024d10: 6865 2070 6f6c 6c20 6f70 7469 6f6e 2079  he poll option y
-00024d20: 6f75 2077 616e 7420 746f 2076 6f74 6520  ou want to vote 
-00024d30: 666f 7220 2830 2074 6f20 3929 2e0a 0a20  for (0 to 9)... 
-00024d40: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00024d50: 2020 2020 2020 2020 2020 2020 3a6f 626a              :obj
-00024d60: 3a60 7e70 7972 6f67 7261 6d2e 7479 7065  :`~pyrogram.type
-00024d70: 732e 506f 6c6c 603a 204f 6e20 7375 6363  s.Poll`: On succ
-00024d80: 6573 732c 2074 6865 2070 6f6c 6c20 7769  ess, the poll wi
-00024d90: 7468 2074 6865 2063 686f 7365 6e20 6f70  th the chosen op
-00024da0: 7469 6f6e 2069 7320 7265 7475 726e 6564  tion is returned
-00024db0: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00024dc0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00024dd0: 5043 4572 726f 723a 2049 6e20 6361 7365  PCError: In case
-00024de0: 206f 6620 6120 5465 6c65 6772 616d 2052   of a Telegram R
-00024df0: 5043 2065 7272 6f72 2e0a 2020 2020 2020  PC error..      
-00024e00: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
-00024e10: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-00024e20: 2e5f 636c 6965 6e74 2e76 6f74 655f 706f  ._client.vote_po
-00024e30: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-00024e40: 6368 6174 5f69 643d 7365 6c66 2e63 6861  chat_id=self.cha
-00024e50: 742e 6964 2c0a 2020 2020 2020 2020 2020  t.id,.          
-00024e60: 2020 6d65 7373 6167 655f 6964 3d73 656c    message_id=sel
-00024e70: 662e 6964 2c0a 2020 2020 2020 2020 2020  f.id,.          
-00024e80: 2020 6f70 7469 6f6e 733d 6f70 7469 6f6e    options=option
-00024e90: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00024ea0: 6173 796e 6320 6465 6620 7069 6e28 7365  async def pin(se
-00024eb0: 6c66 2c20 6469 7361 626c 655f 6e6f 7469  lf, disable_noti
-00024ec0: 6669 6361 7469 6f6e 3a20 626f 6f6c 203d  fication: bool =
-00024ed0: 2046 616c 7365 2c20 626f 7468 5f73 6964   False, both_sid
-00024ee0: 6573 3a20 626f 6f6c 203d 2046 616c 7365  es: bool = False
-00024ef0: 2920 2d3e 2022 7479 7065 732e 4d65 7373  ) -> "types.Mess
-00024f00: 6167 6522 3a0a 2020 2020 2020 2020 2222  age":.        ""
-00024f10: 2242 6f75 6e64 206d 6574 686f 6420 2a70  "Bound method *p
-00024f20: 696e 2a20 6f66 203a 6f62 6a3a 607e 7079  in* of :obj:`~py
-00024f30: 726f 6772 616d 2e74 7970 6573 2e4d 6573  rogram.types.Mes
-00024f40: 7361 6765 602e 0a0a 2020 2020 2020 2020  sage`...        
-00024f50: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
-00024f60: 7420 666f 723a 0a0a 2020 2020 2020 2020  t for:..        
-00024f70: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-00024f80: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-00024f90: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
-00024fa0: 2e70 696e 5f63 6861 745f 6d65 7373 6167  .pin_chat_messag
-00024fb0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00024fc0: 2020 2063 6861 745f 6964 3d6d 6573 7361     chat_id=messa
-00024fd0: 6765 2e63 6861 742e 6964 2c0a 2020 2020  ge.chat.id,.    
-00024fe0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00024ff0: 6167 655f 6964 3d6d 6573 7361 6765 5f69  age_id=message_i
-00025000: 640a 2020 2020 2020 2020 2020 2020 290a  d.            ).
-00025010: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-00025020: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-00025030: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00025040: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-00025050: 2020 2020 2020 6177 6169 7420 6d65 7373        await mess
-00025060: 6167 652e 7069 6e28 290a 0a20 2020 2020  age.pin()..     
-00025070: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
-00025080: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-00025090: 6c65 5f6e 6f74 6966 6963 6174 696f 6e20  le_notification 
-000250a0: 2860 6062 6f6f 6c60 6029 3a0a 2020 2020  (``bool``):.    
-000250b0: 2020 2020 2020 2020 2020 2020 5061 7373              Pass
-000250c0: 2054 7275 652c 2069 6620 6974 2069 7320   True, if it is 
-000250d0: 6e6f 7420 6e65 6365 7373 6172 7920 746f  not necessary to
-000250e0: 2073 656e 6420 6120 6e6f 7469 6669 6361   send a notifica
-000250f0: 7469 6f6e 2074 6f20 616c 6c20 6368 6174  tion to all chat
-00025100: 206d 656d 6265 7273 2061 626f 7574 2074   members about t
-00025110: 6865 206e 6577 2070 696e 6e65 640a 2020  he new pinned.  
-00025120: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00025130: 7373 6167 652e 204e 6f74 6966 6963 6174  ssage. Notificat
-00025140: 696f 6e73 2061 7265 2061 6c77 6179 7320  ions are always 
-00025150: 6469 7361 626c 6564 2069 6e20 6368 616e  disabled in chan
-00025160: 6e65 6c73 2e0a 0a20 2020 2020 2020 2020  nels...         
-00025170: 2020 2062 6f74 685f 7369 6465 7320 2860     both_sides (`
-00025180: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
-00025190: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
-000251a0: 2020 2020 2020 5061 7373 2054 7275 6520        Pass True 
-000251b0: 746f 2070 696e 2074 6865 206d 6573 7361  to pin the messa
-000251c0: 6765 2066 6f72 2062 6f74 6820 7369 6465  ge for both side
-000251d0: 7320 2879 6f75 2061 6e64 2072 6563 6970  s (you and recip
-000251e0: 6965 6e74 292e 0a20 2020 2020 2020 2020  ient)..         
-000251f0: 2020 2020 2020 2041 7070 6c69 6361 626c         Applicabl
-00025200: 6520 746f 2070 7269 7661 7465 2063 6861  e to private cha
-00025210: 7473 206f 6e6c 792e 2044 6566 6175 6c74  ts only. Default
-00025220: 7320 746f 2046 616c 7365 2e0a 0a20 2020  s to False...   
-00025230: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00025240: 2020 2020 2020 2020 2020 3a6f 626a 3a60            :obj:`
-00025250: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
-00025260: 4d65 7373 6167 6560 3a20 4f6e 2073 7563  Message`: On suc
-00025270: 6365 7373 2c20 7468 6520 7365 7276 6963  cess, the servic
-00025280: 6520 6d65 7373 6167 6520 6973 2072 6574  e message is ret
-00025290: 7572 6e65 642e 0a0a 2020 2020 2020 2020  urned...        
-000252a0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-000252b0: 2020 2020 5250 4345 7272 6f72 3a20 496e      RPCError: In
-000252c0: 2063 6173 6520 6f66 2061 2054 656c 6567   case of a Teleg
-000252d0: 7261 6d20 5250 4320 6572 726f 722e 0a20  ram RPC error.. 
-000252e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000252f0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00025300: 7365 6c66 2e5f 636c 6965 6e74 2e70 696e  self._client.pin
-00025310: 5f63 6861 745f 6d65 7373 6167 6528 0a20  _chat_message(. 
-00025320: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-00025330: 6964 3d73 656c 662e 6368 6174 2e69 642c  id=self.chat.id,
-00025340: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
-00025350: 7361 6765 5f69 643d 7365 6c66 2e69 642c  sage_id=self.id,
-00025360: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00025370: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00025380: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
-00025390: 6361 7469 6f6e 2c0a 2020 2020 2020 2020  cation,.        
-000253a0: 2020 2020 626f 7468 5f73 6964 6573 3d62      both_sides=b
-000253b0: 6f74 685f 7369 6465 730a 2020 2020 2020  oth_sides.      
-000253c0: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
-000253d0: 6566 2075 6e70 696e 2873 656c 6629 202d  ef unpin(self) -
-000253e0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-000253f0: 2222 2242 6f75 6e64 206d 6574 686f 6420  """Bound method 
-00025400: 2a75 6e70 696e 2a20 6f66 203a 6f62 6a3a  *unpin* of :obj:
-00025410: 607e 7079 726f 6772 616d 2e74 7970 6573  `~pyrogram.types
-00025420: 2e4d 6573 7361 6765 602e 0a0a 2020 2020  .Message`...    
-00025430: 2020 2020 5573 6520 6173 2061 2073 686f      Use as a sho
-00025440: 7274 6375 7420 666f 723a 0a0a 2020 2020  rtcut for:..    
-00025450: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-00025460: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
-00025470: 2020 2020 2020 2020 6177 6169 7420 636c          await cl
-00025480: 6965 6e74 2e75 6e70 696e 5f63 6861 745f  ient.unpin_chat_
-00025490: 6d65 7373 6167 6528 0a20 2020 2020 2020  message(.       
-000254a0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-000254b0: 3d6d 6573 7361 6765 2e63 6861 742e 6964  =message.chat.id
-000254c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000254d0: 2020 6d65 7373 6167 655f 6964 3d6d 6573    message_id=mes
-000254e0: 7361 6765 5f69 640a 2020 2020 2020 2020  sage_id.        
-000254f0: 2020 2020 290a 0a20 2020 2020 2020 2045      )..        E
-00025500: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
-00025510: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-00025520: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
-00025530: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00025540: 7420 6d65 7373 6167 652e 756e 7069 6e28  t message.unpin(
-00025550: 290a 0a20 2020 2020 2020 2052 6574 7572  )..        Retur
-00025560: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00025570: 5472 7565 206f 6e20 7375 6363 6573 732e  True on success.
-00025580: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
-00025590: 3a0a 2020 2020 2020 2020 2020 2020 5250  :.            RP
-000255a0: 4345 7272 6f72 3a20 496e 2063 6173 6520  CError: In case 
-000255b0: 6f66 2061 2054 656c 6567 7261 6d20 5250  of a Telegram RP
-000255c0: 4320 6572 726f 722e 0a20 2020 2020 2020  C error..       
-000255d0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-000255e0: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
-000255f0: 636c 6965 6e74 2e75 6e70 696e 5f63 6861  client.unpin_cha
-00025600: 745f 6d65 7373 6167 6528 0a20 2020 2020  t_message(.     
-00025610: 2020 2020 2020 2063 6861 745f 6964 3d73         chat_id=s
-00025620: 656c 662e 6368 6174 2e69 642c 0a20 2020  elf.chat.id,.   
-00025630: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00025640: 5f69 643d 7365 6c66 2e69 640a 2020 2020  _id=self.id.    
-00025650: 2020 2020 290a                               ).
+00021ca0: 2020 7175 6573 7469 6f6e 3d73 656c 662e    question=self.
+00021cb0: 706f 6c6c 2e71 7565 7374 696f 6e2c 0a20  poll.question,. 
+00021cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021cd0: 2020 206f 7074 696f 6e73 3d5b 6f70 742e     options=[opt.
+00021ce0: 7465 7874 2066 6f72 206f 7074 2069 6e20  text for opt in 
+00021cf0: 7365 6c66 2e70 6f6c 6c2e 6f70 7469 6f6e  self.poll.option
+00021d00: 735d 2c0a 2020 2020 2020 2020 2020 2020  s],.            
+00021d10: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
+00021d20: 6e6f 7469 6669 6361 7469 6f6e 3d64 6973  notification=dis
+00021d30: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00021d40: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+00021d50: 2020 2020 2020 206d 6573 7361 6765 5f74         message_t
+00021d60: 6872 6561 645f 6964 3d6d 6573 7361 6765  hread_id=message
+00021d70: 5f74 6872 6561 645f 6964 2c0a 2020 2020  _thread_id,.    
+00021d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021d90: 7363 6865 6475 6c65 5f64 6174 653d 7363  schedule_date=sc
+00021da0: 6865 6475 6c65 5f64 6174 650a 2020 2020  hedule_date.    
+00021db0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00021dc0: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
+00021dd0: 656c 662e 6761 6d65 3a0a 2020 2020 2020  elf.game:.      
+00021de0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00021df0: 2061 7761 6974 2073 656c 662e 5f63 6c69   await self._cli
+00021e00: 656e 742e 7365 6e64 5f67 616d 6528 0a20  ent.send_game(. 
+00021e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021e20: 2020 2063 6861 745f 6964 2c0a 2020 2020     chat_id,.    
+00021e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021e40: 6761 6d65 5f73 686f 7274 5f6e 616d 653d  game_short_name=
+00021e50: 7365 6c66 2e67 616d 652e 7368 6f72 745f  self.game.short_
+00021e60: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00021e70: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+00021e80: 655f 6e6f 7469 6669 6361 7469 6f6e 3d64  e_notification=d
+00021e90: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00021ea0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00021eb0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00021ec0: 5f74 6872 6561 645f 6964 3d6d 6573 7361  _thread_id=messa
+00021ed0: 6765 5f74 6872 6561 645f 6964 0a20 2020  ge_thread_id.   
+00021ee0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00021ef0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00021f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021f10: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00021f20: 7228 2255 6e6b 6e6f 776e 206d 6564 6961  r("Unknown media
+00021f30: 2074 7970 6522 290a 0a20 2020 2020 2020   type")..       
+00021f40: 2020 2020 2069 6620 7365 6c66 2e73 7469       if self.sti
+00021f50: 636b 6572 206f 7220 7365 6c66 2e76 6964  cker or self.vid
+00021f60: 656f 5f6e 6f74 653a 2020 2320 5374 6963  eo_note:  # Stic
+00021f70: 6b65 7220 616e 6420 5669 6465 6f4e 6f74  ker and VideoNot
+00021f80: 6520 7368 6f75 6c64 2068 6176 6520 6e6f  e should have no
+00021f90: 2063 6170 7469 6f6e 0a20 2020 2020 2020   caption.       
+00021fa0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00021fb0: 6177 6169 7420 7365 6e64 5f6d 6564 6961  await send_media
+00021fc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00021fd0: 2020 2020 2020 6669 6c65 5f69 643d 6669        file_id=fi
+00021fe0: 6c65 5f69 642c 0a20 2020 2020 2020 2020  le_id,.         
+00021ff0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00022000: 6765 5f74 6872 6561 645f 6964 3d6d 6573  ge_thread_id=mes
+00022010: 7361 6765 5f74 6872 6561 645f 6964 0a20  sage_thread_id. 
+00022020: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00022030: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00022040: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00022050: 2020 2069 6620 6361 7074 696f 6e20 6973     if caption is
+00022060: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00022070: 2020 2020 2020 2020 2020 2063 6170 7469             capti
+00022080: 6f6e 203d 2073 656c 662e 6361 7074 696f  on = self.captio
+00022090: 6e20 6f72 2022 220a 2020 2020 2020 2020  n or "".        
+000220a0: 2020 2020 2020 2020 2020 2020 6361 7074              capt
+000220b0: 696f 6e5f 656e 7469 7469 6573 203d 2073  ion_entities = s
+000220c0: 656c 662e 6361 7074 696f 6e5f 656e 7469  elf.caption_enti
+000220d0: 7469 6573 0a0a 2020 2020 2020 2020 2020  ties..          
+000220e0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+000220f0: 6974 2073 656e 645f 6d65 6469 6128 0a20  it send_media(. 
+00022100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022110: 2020 2066 696c 655f 6964 3d66 696c 655f     file_id=file_
+00022120: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00022130: 2020 2020 2020 2020 6361 7074 696f 6e3d          caption=
+00022140: 6361 7074 696f 6e2c 0a20 2020 2020 2020  caption,.       
+00022150: 2020 2020 2020 2020 2020 2020 2070 6172               par
+00022160: 7365 5f6d 6f64 653d 7061 7273 655f 6d6f  se_mode=parse_mo
+00022170: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
+00022180: 2020 2020 2020 2020 6361 7074 696f 6e5f          caption_
+00022190: 656e 7469 7469 6573 3d63 6170 7469 6f6e  entities=caption
+000221a0: 5f65 6e74 6974 6965 732c 0a20 2020 2020  _entities,.     
+000221b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000221c0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+000221d0: 3d6d 6573 7361 6765 5f74 6872 6561 645f  =message_thread_
+000221e0: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
+000221f0: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
+00022200: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00022210: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00022220: 2243 616e 2774 2063 6f70 7920 7468 6973  "Can't copy this
+00022230: 206d 6573 7361 6765 2229 0a0a 2020 2020   message")..    
+00022240: 6173 796e 6320 6465 6620 6465 6c65 7465  async def delete
+00022250: 2873 656c 662c 2072 6576 6f6b 653a 2062  (self, revoke: b
+00022260: 6f6f 6c20 3d20 5472 7565 293a 0a20 2020  ool = True):.   
+00022270: 2020 2020 2022 2222 426f 756e 6420 6d65       """Bound me
+00022280: 7468 6f64 202a 6465 6c65 7465 2a20 6f66  thod *delete* of
+00022290: 203a 6f62 6a3a 607e 7079 726f 6772 616d   :obj:`~pyrogram
+000222a0: 2e74 7970 6573 2e4d 6573 7361 6765 602e  .types.Message`.
+000222b0: 0a0a 2020 2020 2020 2020 5573 6520 6173  ..        Use as
+000222c0: 2061 2073 686f 7274 6375 7420 666f 723a   a shortcut for:
+000222d0: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
+000222e0: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+000222f0: 0a0a 2020 2020 2020 2020 2020 2020 6177  ..            aw
+00022300: 6169 7420 636c 6965 6e74 2e64 656c 6574  ait client.delet
+00022310: 655f 6d65 7373 6167 6573 280a 2020 2020  e_messages(.    
+00022320: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+00022330: 5f69 643d 6368 6174 5f69 642c 0a20 2020  _id=chat_id,.   
+00022340: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+00022350: 7361 6765 5f69 6473 3d6d 6573 7361 6765  sage_ids=message
+00022360: 2e69 640a 2020 2020 2020 2020 2020 2020  .id.            
+00022370: 290a 0a20 2020 2020 2020 2045 7861 6d70  )..        Examp
+00022380: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00022390: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+000223a0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+000223b0: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
+000223c0: 7373 6167 652e 6465 6c65 7465 2829 0a0a  ssage.delete()..
+000223d0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+000223e0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+000223f0: 7265 766f 6b65 2028 6060 626f 6f6c 6060  revoke (``bool``
+00022400: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
+00022410: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00022420: 656c 6574 6573 206d 6573 7361 6765 7320  eletes messages 
+00022430: 6f6e 2062 6f74 6820 7061 7274 732e 0a20  on both parts.. 
+00022440: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00022450: 6869 7320 6973 206f 6e6c 7920 666f 7220  his is only for 
+00022460: 7072 6976 6174 6520 636c 6f75 6420 6368  private cloud ch
+00022470: 6174 7320 616e 6420 6e6f 726d 616c 2067  ats and normal g
+00022480: 726f 7570 732c 206d 6573 7361 6765 7320  roups, messages 
+00022490: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+000224a0: 2020 2063 6861 6e6e 656c 7320 616e 6420     channels and 
+000224b0: 7375 7065 7267 726f 7570 7320 6172 6520  supergroups are 
+000224c0: 616c 7761 7973 2072 6576 6f6b 6564 2028  always revoked (
+000224d0: 692e 652e 3a20 6465 6c65 7465 6420 666f  i.e.: deleted fo
+000224e0: 7220 6576 6572 796f 6e65 292e 0a20 2020  r everyone)..   
+000224f0: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+00022500: 6175 6c74 7320 746f 2054 7275 652e 0a0a  aults to True...
+00022510: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00022520: 0a20 2020 2020 2020 2020 2020 2054 7275  .            Tru
+00022530: 6520 6f6e 2073 7563 6365 7373 2c20 4661  e on success, Fa
+00022540: 6c73 6520 6f74 6865 7277 6973 652e 0a0a  lse otherwise...
+00022550: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
+00022560: 2020 2020 2020 2020 2020 2020 5250 4345              RPCE
+00022570: 7272 6f72 3a20 496e 2063 6173 6520 6f66  rror: In case of
+00022580: 2061 2054 656c 6567 7261 6d20 5250 4320   a Telegram RPC 
+00022590: 6572 726f 722e 0a20 2020 2020 2020 2022  error..        "
+000225a0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+000225b0: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
+000225c0: 6965 6e74 2e64 656c 6574 655f 6d65 7373  ient.delete_mess
+000225d0: 6167 6573 280a 2020 2020 2020 2020 2020  ages(.          
+000225e0: 2020 6368 6174 5f69 643d 7365 6c66 2e63    chat_id=self.c
+000225f0: 6861 742e 6964 2c0a 2020 2020 2020 2020  hat.id,.        
+00022600: 2020 2020 6d65 7373 6167 655f 6964 733d      message_ids=
+00022610: 7365 6c66 2e69 642c 0a20 2020 2020 2020  self.id,.       
+00022620: 2020 2020 2072 6576 6f6b 653d 7265 766f       revoke=revo
+00022630: 6b65 0a20 2020 2020 2020 2029 0a0a 2020  ke.        )..  
+00022640: 2020 6173 796e 6320 6465 6620 636c 6963    async def clic
+00022650: 6b28 7365 6c66 2c20 783a 2055 6e69 6f6e  k(self, x: Union
+00022660: 5b69 6e74 2c20 7374 725d 203d 2030 2c20  [int, str] = 0, 
+00022670: 793a 2069 6e74 203d 204e 6f6e 652c 2071  y: int = None, q
+00022680: 756f 7465 3a20 626f 6f6c 203d 204e 6f6e  uote: bool = Non
+00022690: 652c 2074 696d 656f 7574 3a20 696e 7420  e, timeout: int 
+000226a0: 3d20 3130 293a 0a20 2020 2020 2020 2022  = 10):.        "
+000226b0: 2222 426f 756e 6420 6d65 7468 6f64 202a  ""Bound method *
+000226c0: 636c 6963 6b2a 206f 6620 3a6f 626a 3a60  click* of :obj:`
+000226d0: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
+000226e0: 4d65 7373 6167 6560 2e0a 0a20 2020 2020  Message`...     
+000226f0: 2020 2055 7365 2061 7320 6120 7368 6f72     Use as a shor
+00022700: 7463 7574 2066 6f72 2063 6c69 636b 696e  tcut for clickin
+00022710: 6720 6120 6275 7474 6f6e 2061 7474 6163  g a button attac
+00022720: 6865 6420 746f 2074 6865 206d 6573 7361  hed to the messa
+00022730: 6765 2069 6e73 7465 6164 206f 663a 0a0a  ge instead of:..
+00022740: 2020 2020 2020 2020 2d20 436c 6963 6b69          - Clicki
+00022750: 6e67 2069 6e6c 696e 6520 6275 7474 6f6e  ng inline button
+00022760: 733a 0a0a 2020 2020 2020 2020 2e2e 2063  s:..        .. c
+00022770: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00022780: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+00022790: 6177 6169 7420 636c 6965 6e74 2e72 6571  await client.req
+000227a0: 7565 7374 5f63 616c 6c62 6163 6b5f 616e  uest_callback_an
+000227b0: 7377 6572 280a 2020 2020 2020 2020 2020  swer(.          
+000227c0: 2020 2020 2020 6368 6174 5f69 643d 6d65        chat_id=me
+000227d0: 7373 6167 652e 6368 6174 2e69 642c 0a20  ssage.chat.id,. 
+000227e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000227f0: 6573 7361 6765 5f69 643d 6d65 7373 6167  essage_id=messag
+00022800: 652e 6964 2c0a 2020 2020 2020 2020 2020  e.id,.          
+00022810: 2020 2020 2020 6361 6c6c 6261 636b 5f64        callback_d
+00022820: 6174 613d 6d65 7373 6167 652e 7265 706c  ata=message.repl
+00022830: 795f 6d61 726b 7570 5b69 5d5b 6a5d 2e63  y_markup[i][j].c
+00022840: 616c 6c62 6163 6b5f 6461 7461 0a20 2020  allback_data.   
+00022850: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00022860: 2020 2020 2d20 436c 6963 6b69 6e67 206e      - Clicking n
+00022870: 6f72 6d61 6c20 6275 7474 6f6e 733a 0a0a  ormal buttons:..
+00022880: 2020 2020 2020 2020 2e2e 2063 6f64 652d          .. code-
+00022890: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+000228a0: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+000228b0: 7420 636c 6965 6e74 2e73 656e 645f 6d65  t client.send_me
+000228c0: 7373 6167 6528 0a20 2020 2020 2020 2020  ssage(.         
+000228d0: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
+000228e0: 6573 7361 6765 2e63 6861 742e 6964 2c0a  essage.chat.id,.
+000228f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022900: 7465 7874 3d6d 6573 7361 6765 2e72 6570  text=message.rep
+00022910: 6c79 5f6d 6172 6b75 705b 695d 5b6a 5d2e  ly_markup[i][j].
+00022920: 7465 7874 0a20 2020 2020 2020 2020 2020  text.           
+00022930: 2029 0a0a 2020 2020 2020 2020 4578 616d   )..        Exam
+00022940: 706c 653a 0a20 2020 2020 2020 2020 2020  ple:.           
+00022950: 2054 6869 7320 6d65 7468 6f64 2063 616e   This method can
+00022960: 2062 6520 7573 6564 2069 6e20 7468 7265   be used in thre
+00022970: 6520 6469 6666 6572 656e 7420 7761 7973  e different ways
+00022980: 3a0a 0a20 2020 2020 2020 2020 2020 2031  :..            1
+00022990: 2e20 2050 6173 7320 6f6e 6520 696e 7465  .  Pass one inte
+000229a0: 6765 7220 6172 6775 6d65 6e74 206f 6e6c  ger argument onl
+000229b0: 7920 2865 2e67 2e3a 2060 602e 636c 6963  y (e.g.: ``.clic
+000229c0: 6b28 3229 6060 2c20 746f 2063 6c69 636b  k(2)``, to click
+000229d0: 2061 2062 7574 746f 6e20 6174 2069 6e64   a button at ind
+000229e0: 6578 2032 292e 0a20 2020 2020 2020 2020  ex 2)..         
+000229f0: 2020 2020 2020 2042 7574 746f 6e73 2061         Buttons a
+00022a00: 7265 2063 6f75 6e74 6564 206c 6566 7420  re counted left 
+00022a10: 746f 2072 6967 6874 2c20 7374 6172 7469  to right, starti
+00022a20: 6e67 2066 726f 6d20 7468 6520 746f 702e  ng from the top.
+00022a30: 0a0a 2020 2020 2020 2020 2020 2020 322e  ..            2.
+00022a40: 2020 5061 7373 2074 776f 2069 6e74 6567    Pass two integ
+00022a50: 6572 2061 7267 756d 656e 7473 2028 652e  er arguments (e.
+00022a60: 672e 3a20 6060 2e63 6c69 636b 2831 2c20  g.: ``.click(1, 
+00022a70: 3029 6060 2c20 746f 2063 6c69 636b 2061  0)``, to click a
+00022a80: 2062 7574 746f 6e20 6174 2070 6f73 6974   button at posit
+00022a90: 696f 6e20 2831 2c20 3029 292e 0a20 2020  ion (1, 0))..   
+00022aa0: 2020 2020 2020 2020 2020 2020 2054 6865               The
+00022ab0: 206f 7269 6769 6e20 2830 2c20 3029 2069   origin (0, 0) i
+00022ac0: 7320 746f 702d 6c65 6674 2e0a 0a20 2020  s top-left...   
+00022ad0: 2020 2020 2020 2020 2033 2e20 2050 6173           3.  Pas
+00022ae0: 7320 6f6e 6520 7374 7269 6e67 2061 7267  s one string arg
+00022af0: 756d 656e 7420 6f6e 6c79 2028 652e 672e  ument only (e.g.
+00022b00: 3a20 6060 2e63 6c69 636b 2822 5365 7474  : ``.click("Sett
+00022b10: 696e 6773 2229 6060 2c20 746f 2063 6c69  ings")``, to cli
+00022b20: 636b 2061 2062 7574 746f 6e20 6279 2075  ck a button by u
+00022b30: 7369 6e67 2069 7473 206c 6162 656c 292e  sing its label).
+00022b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022b50: 204f 6e6c 7920 7468 6520 6669 7273 7420   Only the first 
+00022b60: 6d61 7463 6869 6e67 2062 7574 746f 6e20  matching button 
+00022b70: 7769 6c6c 2062 6520 7072 6573 7365 642e  will be pressed.
+00022b80: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00022b90: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
+00022ba0: 2020 7820 2860 6069 6e74 6060 207c 2060    x (``int`` | `
+00022bb0: 6073 7472 6060 293a 0a20 2020 2020 2020  `str``):.       
+00022bc0: 2020 2020 2020 2020 2055 7365 6420 6173           Used as
+00022bd0: 2069 6e74 6567 6572 2069 6e64 6578 2c20   integer index, 
+00022be0: 696e 7465 6765 7220 6162 7363 6973 7361  integer abscissa
+00022bf0: 2028 696e 2070 6169 7220 7769 7468 2079   (in pair with y
+00022c00: 2920 6f72 2061 7320 7374 7269 6e67 206c  ) or as string l
+00022c10: 6162 656c 2e0a 2020 2020 2020 2020 2020  abel..          
+00022c20: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+00022c30: 6f20 3020 2866 6972 7374 2062 7574 746f  o 0 (first butto
+00022c40: 6e29 2e0a 0a20 2020 2020 2020 2020 2020  n)...           
+00022c50: 2079 2028 6060 696e 7460 602c 202a 6f70   y (``int``, *op
+00022c60: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
+00022c70: 2020 2020 2020 2020 2020 5573 6564 2061            Used a
+00022c80: 7320 6f72 6469 6e61 7465 206f 6e6c 7920  s ordinate only 
+00022c90: 2869 6e20 7061 6972 2077 6974 6820 7829  (in pair with x)
+00022ca0: 2e0a 0a20 2020 2020 2020 2020 2020 2071  ...            q
+00022cb0: 756f 7465 2028 6060 626f 6f6c 6060 2c20  uote (``bool``, 
+00022cc0: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
+00022cd0: 2020 2020 2020 2020 2020 2020 2055 7365               Use
+00022ce0: 6675 6c20 666f 7220 6e6f 726d 616c 2062  ful for normal b
+00022cf0: 7574 746f 6e73 206f 6e6c 792c 2077 6865  uttons only, whe
+00022d00: 7265 2070 7265 7373 696e 6720 6974 2077  re pressing it w
+00022d10: 696c 6c20 7265 7375 6c74 2069 6e20 6120  ill result in a 
+00022d20: 6e65 7720 6d65 7373 6167 6520 7365 6e74  new message sent
+00022d30: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00022d40: 2020 4966 2060 6054 7275 6560 602c 2074    If ``True``, t
+00022d50: 6865 206d 6573 7361 6765 2077 696c 6c20  he message will 
+00022d60: 6265 2073 656e 7420 6173 2061 2072 6570  be sent as a rep
+00022d70: 6c79 2074 6f20 7468 6973 206d 6573 7361  ly to this messa
+00022d80: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
+00022d90: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00022da0: 6060 5472 7565 6060 2069 6e20 6772 6f75  ``True`` in grou
+00022db0: 7020 6368 6174 7320 616e 6420 6060 4661  p chats and ``Fa
+00022dc0: 6c73 6560 6020 696e 2070 7269 7661 7465  lse`` in private
+00022dd0: 2063 6861 7473 2e0a 0a20 2020 2020 2020   chats...       
+00022de0: 2020 2020 2074 696d 656f 7574 2028 6060       timeout (``
+00022df0: 696e 7460 602c 202a 6f70 7469 6f6e 616c  int``, *optional
+00022e00: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
+00022e10: 2020 2020 5469 6d65 6f75 7420 696e 2073      Timeout in s
+00022e20: 6563 6f6e 6473 2e0a 0a20 2020 2020 2020  econds...       
+00022e30: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00022e40: 2020 2020 2020 2d20 2020 5468 6520 7265        -   The re
+00022e50: 7375 6c74 206f 6620 3a6d 6574 683a 607e  sult of :meth:`~
+00022e60: 7079 726f 6772 616d 2e43 6c69 656e 742e  pyrogram.Client.
+00022e70: 7265 7175 6573 745f 6361 6c6c 6261 636b  request_callback
+00022e80: 5f61 6e73 7765 7260 2069 6e20 6361 7365  _answer` in case
+00022e90: 206f 6620 696e 6c69 6e65 2063 616c 6c62   of inline callb
+00022ea0: 6163 6b20 6275 7474 6f6e 2063 6c69 636b  ack button click
+00022eb0: 732e 0a20 2020 2020 2020 2020 2020 202d  s..            -
+00022ec0: 2020 2054 6865 2072 6573 756c 7420 6f66     The result of
+00022ed0: 203a 6d65 7468 3a60 7e4d 6573 7361 6765   :meth:`~Message
+00022ee0: 2e72 6570 6c79 2829 6020 696e 2063 6173  .reply()` in cas
+00022ef0: 6520 6f66 206e 6f72 6d61 6c20 6275 7474  e of normal butt
+00022f00: 6f6e 2063 6c69 636b 732e 0a20 2020 2020  on clicks..     
+00022f10: 2020 2020 2020 202d 2020 2041 2073 7472         -   A str
+00022f20: 696e 6720 696e 2063 6173 6520 7468 6520  ing in case the 
+00022f30: 696e 6c69 6e65 2062 7574 746f 6e20 6973  inline button is
+00022f40: 2061 2055 524c 2c20 6120 2a73 7769 7463   a URL, a *switc
+00022f50: 685f 696e 6c69 6e65 5f71 7565 7279 2a20  h_inline_query* 
+00022f60: 6f72 2061 0a20 2020 2020 2020 2020 2020  or a.           
+00022f70: 2020 2020 202a 7377 6974 6368 5f69 6e6c       *switch_inl
+00022f80: 696e 655f 7175 6572 795f 6375 7272 656e  ine_query_curren
+00022f90: 745f 6368 6174 2a20 6275 7474 6f6e 2e0a  t_chat* button..
+00022fa0: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+00022fb0: 0a20 2020 2020 2020 2020 2020 2052 5043  .            RPC
+00022fc0: 4572 726f 723a 2049 6e20 6361 7365 206f  Error: In case o
+00022fd0: 6620 6120 5465 6c65 6772 616d 2052 5043  f a Telegram RPC
+00022fe0: 2065 7272 6f72 2e0a 2020 2020 2020 2020   error..        
+00022ff0: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
+00023000: 496e 2063 6173 6520 7468 6520 7072 6f76  In case the prov
+00023010: 6964 6564 2069 6e64 6578 206f 7220 706f  ided index or po
+00023020: 7369 7469 6f6e 2069 7320 6f75 7420 6f66  sition is out of
+00023030: 2072 616e 6765 206f 7220 7468 6520 6275   range or the bu
+00023040: 7474 6f6e 206c 6162 656c 2077 6173 206e  tton label was n
+00023050: 6f74 2066 6f75 6e64 2e0a 2020 2020 2020  ot found..      
+00023060: 2020 2020 2020 5469 6d65 6f75 7445 7272        TimeoutErr
+00023070: 6f72 3a20 496e 2063 6173 652c 2061 6674  or: In case, aft
+00023080: 6572 2063 6c69 636b 696e 6720 616e 2069  er clicking an i
+00023090: 6e6c 696e 6520 6275 7474 6f6e 2c20 7468  nline button, th
+000230a0: 6520 626f 7420 6661 696c 7320 746f 2061  e bot fails to a
+000230b0: 6e73 7765 7220 7769 7468 696e 2074 6865  nswer within the
+000230c0: 2074 696d 656f 7574 2e0a 2020 2020 2020   timeout..      
+000230d0: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
+000230e0: 6620 6973 696e 7374 616e 6365 2873 656c  f isinstance(sel
+000230f0: 662e 7265 706c 795f 6d61 726b 7570 2c20  f.reply_markup, 
+00023100: 7479 7065 732e 5265 706c 794b 6579 626f  types.ReplyKeybo
+00023110: 6172 644d 6172 6b75 7029 3a0a 2020 2020  ardMarkup):.    
+00023120: 2020 2020 2020 2020 6b65 7962 6f61 7264          keyboard
+00023130: 203d 2073 656c 662e 7265 706c 795f 6d61   = self.reply_ma
+00023140: 726b 7570 2e6b 6579 626f 6172 640a 2020  rkup.keyboard.  
+00023150: 2020 2020 2020 2020 2020 6973 5f69 6e6c            is_inl
+00023160: 696e 6520 3d20 4661 6c73 650a 2020 2020  ine = False.    
+00023170: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+00023180: 6e63 6528 7365 6c66 2e72 6570 6c79 5f6d  nce(self.reply_m
+00023190: 6172 6b75 702c 2074 7970 6573 2e49 6e6c  arkup, types.Inl
+000231a0: 696e 654b 6579 626f 6172 644d 6172 6b75  ineKeyboardMarku
+000231b0: 7029 3a0a 2020 2020 2020 2020 2020 2020  p):.            
+000231c0: 6b65 7962 6f61 7264 203d 2073 656c 662e  keyboard = self.
+000231d0: 7265 706c 795f 6d61 726b 7570 2e69 6e6c  reply_markup.inl
+000231e0: 696e 655f 6b65 7962 6f61 7264 0a20 2020  ine_keyboard.   
+000231f0: 2020 2020 2020 2020 2069 735f 696e 6c69           is_inli
+00023200: 6e65 203d 2054 7275 650a 2020 2020 2020  ne = True.      
+00023210: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00023220: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00023230: 7272 6f72 2822 5468 6520 6d65 7373 6167  rror("The messag
+00023240: 6520 646f 6573 6e27 7420 636f 6e74 6169  e doesn't contai
+00023250: 6e20 616e 7920 6b65 7962 6f61 7264 2229  n any keyboard")
+00023260: 0a0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
+00023270: 6e73 7461 6e63 6528 782c 2069 6e74 2920  nstance(x, int) 
+00023280: 616e 6420 7920 6973 204e 6f6e 653a 0a20  and y is None:. 
+00023290: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+000232a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000232b0: 6275 7474 6f6e 203d 205b 0a20 2020 2020  button = [.     
+000232c0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+000232d0: 7574 746f 6e0a 2020 2020 2020 2020 2020  utton.          
+000232e0: 2020 2020 2020 2020 2020 666f 7220 726f            for ro
+000232f0: 7720 696e 206b 6579 626f 6172 640a 2020  w in keyboard.  
+00023300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023310: 2020 666f 7220 6275 7474 6f6e 2069 6e20    for button in 
+00023320: 726f 770a 2020 2020 2020 2020 2020 2020  row.            
+00023330: 2020 2020 5d5b 785d 0a20 2020 2020 2020      ][x].       
+00023340: 2020 2020 2065 7863 6570 7420 496e 6465       except Inde
+00023350: 7845 7272 6f72 3a0a 2020 2020 2020 2020  xError:.        
+00023360: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00023370: 6c75 6545 7272 6f72 2866 2254 6865 2062  lueError(f"The b
+00023380: 7574 746f 6e20 6174 2069 6e64 6578 207b  utton at index {
+00023390: 787d 2064 6f65 736e 2774 2065 7869 7374  x} doesn't exist
+000233a0: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
+000233b0: 6973 696e 7374 616e 6365 2878 2c20 696e  isinstance(x, in
+000233c0: 7429 2061 6e64 2069 7369 6e73 7461 6e63  t) and isinstanc
+000233d0: 6528 792c 2069 6e74 293a 0a20 2020 2020  e(y, int):.     
+000233e0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+000233f0: 2020 2020 2020 2020 2020 2020 6275 7474              butt
+00023400: 6f6e 203d 206b 6579 626f 6172 645b 795d  on = keyboard[y]
+00023410: 5b78 5d0a 2020 2020 2020 2020 2020 2020  [x].            
+00023420: 6578 6365 7074 2049 6e64 6578 4572 726f  except IndexErro
+00023430: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+00023440: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00023450: 726f 7228 6622 5468 6520 6275 7474 6f6e  ror(f"The button
+00023460: 2061 7420 706f 7369 7469 6f6e 2028 7b78   at position ({x
+00023470: 7d2c 207b 797d 2920 646f 6573 6e27 7420  }, {y}) doesn't 
+00023480: 6578 6973 7422 290a 2020 2020 2020 2020  exist").        
+00023490: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+000234a0: 782c 2073 7472 2920 616e 6420 7920 6973  x, str) and y is
+000234b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000234c0: 2020 206c 6162 656c 203d 2078 2e65 6e63     label = x.enc
+000234d0: 6f64 6528 2275 7466 2d31 3622 2c20 2273  ode("utf-16", "s
+000234e0: 7572 726f 6761 7465 7061 7373 2229 2e64  urrogatepass").d
+000234f0: 6563 6f64 6528 2275 7466 2d31 3622 290a  ecode("utf-16").
+00023500: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00023510: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00023520: 2020 6275 7474 6f6e 203d 205b 0a20 2020    button = [.   
+00023530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023540: 2062 7574 746f 6e0a 2020 2020 2020 2020   button.        
+00023550: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00023560: 726f 7720 696e 206b 6579 626f 6172 640a  row in keyboard.
+00023570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023580: 2020 2020 666f 7220 6275 7474 6f6e 2069      for button i
+00023590: 6e20 726f 770a 2020 2020 2020 2020 2020  n row.          
+000235a0: 2020 2020 2020 2020 2020 6966 206c 6162            if lab
+000235b0: 656c 203d 3d20 6275 7474 6f6e 2e74 6578  el == button.tex
+000235c0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+000235d0: 2020 5d5b 305d 0a20 2020 2020 2020 2020    ][0].         
+000235e0: 2020 2065 7863 6570 7420 496e 6465 7845     except IndexE
+000235f0: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+00023600: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00023610: 6545 7272 6f72 2866 2254 6865 2062 7574  eError(f"The but
+00023620: 746f 6e20 7769 7468 206c 6162 656c 2027  ton with label '
+00023630: 7b78 7d27 2064 6f65 736e 2774 2065 7869  {x}' doesn't exi
+00023640: 7374 7322 290a 2020 2020 2020 2020 656c  sts").        el
+00023650: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00023660: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00023670: 2822 496e 7661 6c69 6420 6172 6775 6d65  ("Invalid argume
+00023680: 6e74 7322 290a 0a20 2020 2020 2020 2069  nts")..        i
+00023690: 6620 6973 5f69 6e6c 696e 653a 0a20 2020  f is_inline:.   
+000236a0: 2020 2020 2020 2020 2069 6620 6275 7474           if butt
+000236b0: 6f6e 2e63 616c 6c62 6163 6b5f 6461 7461  on.callback_data
+000236c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000236d0: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+000236e0: 656c 662e 5f63 6c69 656e 742e 7265 7175  elf._client.requ
+000236f0: 6573 745f 6361 6c6c 6261 636b 5f61 6e73  est_callback_ans
+00023700: 7765 7228 0a20 2020 2020 2020 2020 2020  wer(.           
+00023710: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+00023720: 3d73 656c 662e 6368 6174 2e69 642c 0a20  =self.chat.id,. 
+00023730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023740: 2020 206d 6573 7361 6765 5f69 643d 7365     message_id=se
+00023750: 6c66 2e69 642c 0a20 2020 2020 2020 2020  lf.id,.         
+00023760: 2020 2020 2020 2020 2020 2063 616c 6c62             callb
+00023770: 6163 6b5f 6461 7461 3d62 7574 746f 6e2e  ack_data=button.
+00023780: 6361 6c6c 6261 636b 5f64 6174 612c 0a20  callback_data,. 
+00023790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000237a0: 2020 2074 696d 656f 7574 3d74 696d 656f     timeout=timeo
+000237b0: 7574 0a20 2020 2020 2020 2020 2020 2020  ut.             
+000237c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000237d0: 2065 6c69 6620 6275 7474 6f6e 2e75 726c   elif button.url
+000237e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000237f0: 2020 7265 7475 726e 2062 7574 746f 6e2e    return button.
+00023800: 7572 6c0a 2020 2020 2020 2020 2020 2020  url.            
+00023810: 656c 6966 2062 7574 746f 6e2e 7377 6974  elif button.swit
+00023820: 6368 5f69 6e6c 696e 655f 7175 6572 793a  ch_inline_query:
+00023830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023840: 2072 6574 7572 6e20 6275 7474 6f6e 2e73   return button.s
+00023850: 7769 7463 685f 696e 6c69 6e65 5f71 7565  witch_inline_que
+00023860: 7279 0a20 2020 2020 2020 2020 2020 2065  ry.            e
+00023870: 6c69 6620 6275 7474 6f6e 2e73 7769 7463  lif button.switc
+00023880: 685f 696e 6c69 6e65 5f71 7565 7279 5f63  h_inline_query_c
+00023890: 7572 7265 6e74 5f63 6861 743a 0a20 2020  urrent_chat:.   
+000238a0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000238b0: 7572 6e20 6275 7474 6f6e 2e73 7769 7463  urn button.switc
+000238c0: 685f 696e 6c69 6e65 5f71 7565 7279 5f63  h_inline_query_c
+000238d0: 7572 7265 6e74 5f63 6861 740a 2020 2020  urrent_chat.    
+000238e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000238f0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00023900: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00023910: 5468 6973 2062 7574 746f 6e20 6973 206e  This button is n
+00023920: 6f74 2073 7570 706f 7274 6564 2079 6574  ot supported yet
+00023930: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
+00023940: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
+00023950: 6974 2073 656c 662e 7265 706c 7928 6275  it self.reply(bu
+00023960: 7474 6f6e 2c20 7175 6f74 653d 7175 6f74  tton, quote=quot
+00023970: 6529 0a0a 2020 2020 6173 796e 6320 6465  e)..    async de
+00023980: 6620 7265 6163 7428 7365 6c66 2c20 656d  f react(self, em
+00023990: 6f6a 693a 2073 7472 203d 2022 222c 2062  oji: str = "", b
+000239a0: 6967 3a20 626f 6f6c 203d 2046 616c 7365  ig: bool = False
+000239b0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+000239c0: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
+000239d0: 6f64 202a 7265 6163 742a 206f 6620 3a6f  od *react* of :o
+000239e0: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
+000239f0: 7065 732e 4d65 7373 6167 6560 2e0a 0a20  pes.Message`... 
+00023a00: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
+00023a10: 7368 6f72 7463 7574 2066 6f72 3a0a 0a20  shortcut for:.. 
+00023a20: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+00023a30: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+00023a40: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00023a50: 2063 6c69 656e 742e 7365 6e64 5f72 6561   client.send_rea
+00023a60: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
+00023a70: 2020 2020 2020 2063 6861 745f 6964 3d63         chat_id=c
+00023a80: 6861 745f 6964 2c0a 2020 2020 2020 2020  hat_id,.        
+00023a90: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+00023aa0: 6964 3d6d 6573 7361 6765 2e69 642c 0a20  id=message.id,. 
+00023ab0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00023ac0: 6d6f 6a69 3d22 f09f 94a5 220a 2020 2020  moji="....".    
+00023ad0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00023ae0: 2020 2045 7861 6d70 6c65 3a0a 2020 2020     Example:.    
+00023af0: 2020 2020 2020 2020 2e2e 2063 6f64 652d          .. code-
+00023b00: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+00023b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b20: 6177 6169 7420 6d65 7373 6167 652e 7265  await message.re
+00023b30: 6163 7428 656d 6f6a 693d 22f0 9f94 a522  act(emoji="...."
+00023b40: 290a 0a20 2020 2020 2020 2050 6172 616d  )..        Param
+00023b50: 6574 6572 733a 0a20 2020 2020 2020 2020  eters:.         
+00023b60: 2020 2065 6d6f 6a69 2028 6060 7374 7260     emoji (``str`
+00023b70: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+00023b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b90: 5265 6163 7469 6f6e 2065 6d6f 6a69 2e0a  Reaction emoji..
+00023ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023bb0: 5061 7373 2022 2220 6173 2065 6d6f 6a69  Pass "" as emoji
+00023bc0: 2028 6465 6661 756c 7429 2074 6f20 7265   (default) to re
+00023bd0: 7472 6163 7420 7468 6520 7265 6163 7469  tract the reacti
+00023be0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+00023bf0: 200a 2020 2020 2020 2020 2020 2020 6269   .            bi
+00023c00: 6720 2860 6062 6f6f 6c60 602c 202a 6f70  g (``bool``, *op
+00023c10: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
+00023c20: 2020 2020 2020 2020 2020 5061 7373 2054            Pass T
+00023c30: 7275 6520 746f 2073 686f 7720 6120 6269  rue to show a bi
+00023c40: 6767 6572 2061 6e64 206c 6f6e 6765 7220  gger and longer 
+00023c50: 7265 6163 7469 6f6e 2e0a 2020 2020 2020  reaction..      
+00023c60: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00023c70: 7473 2074 6f20 4661 6c73 652e 0a0a 2020  ts to False...  
+00023c80: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00023c90: 2020 2020 2020 2020 2020 2060 6062 6f6f             ``boo
+00023ca0: 6c60 603a 204f 6e20 7375 6363 6573 732c  l``: On success,
+00023cb0: 2054 7275 6520 6973 2072 6574 7572 6e65   True is returne
+00023cc0: 642e 0a0a 2020 2020 2020 2020 5261 6973  d...        Rais
+00023cd0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00023ce0: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
+00023cf0: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
+00023d00: 5250 4320 6572 726f 722e 0a20 2020 2020  RPC error..     
+00023d10: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00023d20: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+00023d30: 662e 5f63 6c69 656e 742e 7365 6e64 5f72  f._client.send_r
+00023d40: 6561 6374 696f 6e28 0a20 2020 2020 2020  eaction(.       
+00023d50: 2020 2020 2063 6861 745f 6964 3d73 656c       chat_id=sel
+00023d60: 662e 6368 6174 2e69 642c 0a20 2020 2020  f.chat.id,.     
+00023d70: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
+00023d80: 643d 7365 6c66 2e69 642c 0a20 2020 2020  d=self.id,.     
+00023d90: 2020 2020 2020 2065 6d6f 6a69 3d65 6d6f         emoji=emo
+00023da0: 6a69 2c0a 2020 2020 2020 2020 2020 2020  ji,.            
+00023db0: 6269 673d 6269 670a 2020 2020 2020 2020  big=big.        
+00023dc0: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+00023dd0: 2072 6574 7261 6374 5f76 6f74 6528 0a20   retract_vote(. 
+00023de0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00023df0: 2029 202d 3e20 2274 7970 6573 2e50 6f6c   ) -> "types.Pol
+00023e00: 6c22 3a0a 2020 2020 2020 2020 2222 2242  l":.        """B
+00023e10: 6f75 6e64 206d 6574 686f 6420 2a72 6574  ound method *ret
+00023e20: 7261 6374 5f76 6f74 652a 206f 6620 3a6f  ract_vote* of :o
+00023e30: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
+00023e40: 7065 732e 4d65 7373 6167 6560 2e0a 0a20  pes.Message`... 
+00023e50: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
+00023e60: 7368 6f72 7463 7574 2066 6f72 3a0a 0a20  shortcut for:.. 
+00023e70: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+00023e80: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+00023e90: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
+00023ea0: 742e 7265 7472 6163 745f 766f 7465 280a  t.retract_vote(.
+00023eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ec0: 6368 6174 5f69 643d 6d65 7373 6167 652e  chat_id=message.
+00023ed0: 6368 6174 2e69 642c 0a20 2020 2020 2020  chat.id,.       
+00023ee0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00023ef0: 5f69 643d 6d65 7373 6167 655f 6964 2c0a  _id=message_id,.
+00023f00: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00023f10: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
+00023f20: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
+00023f30: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00023f40: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+00023f50: 2020 2020 6d65 7373 6167 652e 7265 7472      message.retr
+00023f60: 6163 745f 766f 7465 2829 0a0a 2020 2020  act_vote()..    
+00023f70: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00023f80: 2020 2020 2020 2020 203a 6f62 6a3a 607e           :obj:`~
+00023f90: 7079 726f 6772 616d 2e74 7970 6573 2e50  pyrogram.types.P
+00023fa0: 6f6c 6c60 3a20 4f6e 2073 7563 6365 7373  oll`: On success
+00023fb0: 2c20 7468 6520 706f 6c6c 2077 6974 6820  , the poll with 
+00023fc0: 7468 6520 7265 7472 6163 7465 6420 766f  the retracted vo
+00023fd0: 7465 2069 7320 7265 7475 726e 6564 2e0a  te is returned..
+00023fe0: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+00023ff0: 0a20 2020 2020 2020 2020 2020 2052 5043  .            RPC
+00024000: 4572 726f 723a 2049 6e20 6361 7365 206f  Error: In case o
+00024010: 6620 6120 5465 6c65 6772 616d 2052 5043  f a Telegram RPC
+00024020: 2065 7272 6f72 2e0a 2020 2020 2020 2020   error..        
+00024030: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+00024040: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
+00024050: 636c 6965 6e74 2e72 6574 7261 6374 5f76  client.retract_v
+00024060: 6f74 6528 0a20 2020 2020 2020 2020 2020  ote(.           
+00024070: 2063 6861 745f 6964 3d73 656c 662e 6368   chat_id=self.ch
+00024080: 6174 2e69 642c 0a20 2020 2020 2020 2020  at.id,.         
+00024090: 2020 206d 6573 7361 6765 5f69 643d 7365     message_id=se
+000240a0: 6c66 2e69 640a 2020 2020 2020 2020 290a  lf.id.        ).
+000240b0: 0a20 2020 2061 7379 6e63 2064 6566 2064  .    async def d
+000240c0: 6f77 6e6c 6f61 6428 0a20 2020 2020 2020  ownload(.       
+000240d0: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
+000240e0: 696c 655f 6e61 6d65 3a20 7374 7220 3d20  ile_name: str = 
+000240f0: 2222 2c0a 2020 2020 2020 2020 696e 5f6d  "",.        in_m
+00024100: 656d 6f72 793a 2062 6f6f 6c20 3d20 4661  emory: bool = Fa
+00024110: 6c73 652c 0a20 2020 2020 2020 2062 6c6f  lse,.        blo
+00024120: 636b 3a20 626f 6f6c 203d 2054 7275 652c  ck: bool = True,
+00024130: 0a20 2020 2020 2020 2070 726f 6772 6573  .        progres
+00024140: 733a 2043 616c 6c61 626c 6520 3d20 4e6f  s: Callable = No
+00024150: 6e65 2c0a 2020 2020 2020 2020 7072 6f67  ne,.        prog
+00024160: 7265 7373 5f61 7267 733a 2074 7570 6c65  ress_args: tuple
+00024170: 203d 2028 290a 2020 2020 2920 2d3e 2073   = ().    ) -> s
+00024180: 7472 3a0a 2020 2020 2020 2020 2222 2242  tr:.        """B
+00024190: 6f75 6e64 206d 6574 686f 6420 2a64 6f77  ound method *dow
+000241a0: 6e6c 6f61 642a 206f 6620 3a6f 626a 3a60  nload* of :obj:`
+000241b0: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
+000241c0: 4d65 7373 6167 6560 2e0a 0a20 2020 2020  Message`...     
+000241d0: 2020 2055 7365 2061 7320 6120 7368 6f72     Use as a shor
+000241e0: 7463 7574 2066 6f72 3a0a 0a20 2020 2020  tcut for:..     
+000241f0: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+00024200: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+00024210: 2020 2020 2020 2061 7761 6974 2063 6c69         await cli
+00024220: 656e 742e 646f 776e 6c6f 6164 5f6d 6564  ent.download_med
+00024230: 6961 286d 6573 7361 6765 290a 0a20 2020  ia(message)..   
+00024240: 2020 2020 2045 7861 6d70 6c65 3a0a 2020       Example:.  
+00024250: 2020 2020 2020 2020 2020 2e2e 2063 6f64            .. cod
+00024260: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+00024270: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00024280: 2020 6177 6169 7420 6d65 7373 6167 652e    await message.
+00024290: 646f 776e 6c6f 6164 2829 0a0a 2020 2020  download()..    
+000242a0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
+000242b0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+000242c0: 5f6e 616d 6520 2860 6073 7472 6060 2c20  _name (``str``, 
+000242d0: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
+000242e0: 2020 2020 2020 2020 2020 2020 2041 2063               A c
+000242f0: 7573 746f 6d20 2a66 696c 655f 6e61 6d65  ustom *file_name
+00024300: 2a20 746f 2062 6520 7573 6564 2069 6e73  * to be used ins
+00024310: 7465 6164 206f 6620 7468 6520 6f6e 6520  tead of the one 
+00024320: 7072 6f76 6964 6564 2062 7920 5465 6c65  provided by Tele
+00024330: 6772 616d 2e0a 2020 2020 2020 2020 2020  gram..          
+00024340: 2020 2020 2020 4279 2064 6566 6175 6c74        By default
+00024350: 2c20 616c 6c20 6669 6c65 7320 6172 6520  , all files are 
+00024360: 646f 776e 6c6f 6164 6564 2069 6e20 7468  downloaded in th
+00024370: 6520 2a64 6f77 6e6c 6f61 6473 2a20 666f  e *downloads* fo
+00024380: 6c64 6572 2069 6e20 796f 7572 2077 6f72  lder in your wor
+00024390: 6b69 6e67 2064 6972 6563 746f 7279 2e0a  king directory..
+000243a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000243b0: 596f 7520 6361 6e20 616c 736f 2073 7065  You can also spe
+000243c0: 6369 6679 2061 2070 6174 6820 666f 7220  cify a path for 
+000243d0: 646f 776e 6c6f 6164 696e 6720 6669 6c65  downloading file
+000243e0: 7320 696e 2061 2063 7573 746f 6d20 6c6f  s in a custom lo
+000243f0: 6361 7469 6f6e 3a20 7061 7468 7320 7468  cation: paths th
+00024400: 6174 2065 6e64 2077 6974 6820 222f 220a  at end with "/".
+00024410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024420: 6172 6520 636f 6e73 6964 6572 6564 2064  are considered d
+00024430: 6972 6563 746f 7269 6573 2e20 416c 6c20  irectories. All 
+00024440: 6e6f 6e2d 6578 6973 7465 6e74 2066 6f6c  non-existent fol
+00024450: 6465 7273 2077 696c 6c20 6265 2063 7265  ders will be cre
+00024460: 6174 6564 2061 7574 6f6d 6174 6963 616c  ated automatical
+00024470: 6c79 2e0a 0a20 2020 2020 2020 2020 2020  ly...           
+00024480: 2069 6e5f 6d65 6d6f 7279 2028 6060 626f   in_memory (``bo
+00024490: 6f6c 6060 2c20 2a6f 7074 696f 6e61 6c2a  ol``, *optional*
+000244a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000244b0: 2020 2050 6173 7320 5472 7565 2074 6f20     Pass True to 
+000244c0: 646f 776e 6c6f 6164 2074 6865 206d 6564  download the med
+000244d0: 6961 2069 6e2d 6d65 6d6f 7279 2e0a 2020  ia in-memory..  
+000244e0: 2020 2020 2020 2020 2020 2020 2020 4120                A 
+000244f0: 6269 6e61 7279 2066 696c 652d 6c69 6b65  binary file-like
+00024500: 206f 626a 6563 7420 7769 7468 2069 7473   object with its
+00024510: 2061 7474 7269 6275 7465 2022 2e6e 616d   attribute ".nam
+00024520: 6522 2073 6574 2077 696c 6c20 6265 2072  e" set will be r
+00024530: 6574 7572 6e65 642e 0a20 2020 2020 2020  eturned..       
+00024540: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+00024550: 7320 746f 2046 616c 7365 2e0a 0a20 2020  s to False...   
+00024560: 2020 2020 2020 2020 2062 6c6f 636b 2028           block (
+00024570: 6060 626f 6f6c 6060 2c20 2a6f 7074 696f  ``bool``, *optio
+00024580: 6e61 6c2a 293a 0a20 2020 2020 2020 2020  nal*):.         
+00024590: 2020 2020 2020 2042 6c6f 636b 7320 7468         Blocks th
+000245a0: 6520 636f 6465 2065 7865 6375 7469 6f6e  e code execution
+000245b0: 2075 6e74 696c 2074 6865 2066 696c 6520   until the file 
+000245c0: 6861 7320 6265 656e 2064 6f77 6e6c 6f61  has been downloa
+000245d0: 6465 642e 0a20 2020 2020 2020 2020 2020  ded..           
+000245e0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+000245f0: 2054 7275 652e 0a0a 2020 2020 2020 2020   True...        
+00024600: 2020 2020 7072 6f67 7265 7373 2028 6060      progress (``
+00024610: 4361 6c6c 6162 6c65 6060 2c20 2a6f 7074  Callable``, *opt
+00024620: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
+00024630: 2020 2020 2020 2020 2050 6173 7320 6120           Pass a 
+00024640: 6361 6c6c 6261 636b 2066 756e 6374 696f  callback functio
+00024650: 6e20 746f 2076 6965 7720 7468 6520 6669  n to view the fi
+00024660: 6c65 2074 7261 6e73 6d69 7373 696f 6e20  le transmission 
+00024670: 7072 6f67 7265 7373 2e0a 2020 2020 2020  progress..      
+00024680: 2020 2020 2020 2020 2020 5468 6520 6675            The fu
+00024690: 6e63 7469 6f6e 206d 7573 7420 7461 6b65  nction must take
+000246a0: 202a 2863 7572 7265 6e74 2c20 746f 7461   *(current, tota
+000246b0: 6c29 2a20 6173 2070 6f73 6974 696f 6e61  l)* as positiona
+000246c0: 6c20 6172 6775 6d65 6e74 7320 286c 6f6f  l arguments (loo
+000246d0: 6b20 6174 204f 7468 6572 2050 6172 616d  k at Other Param
+000246e0: 6574 6572 7320 6265 6c6f 7720 666f 7220  eters below for 
+000246f0: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00024700: 2020 6465 7461 696c 6564 2064 6573 6372    detailed descr
+00024710: 6970 7469 6f6e 2920 616e 6420 7769 6c6c  iption) and will
+00024720: 2062 6520 6361 6c6c 6564 2062 6163 6b20   be called back 
+00024730: 6561 6368 2074 696d 6520 6120 6e65 7720  each time a new 
+00024740: 6669 6c65 2063 6875 6e6b 2068 6173 2062  file chunk has b
+00024750: 6565 6e20 7375 6363 6573 7366 756c 6c79  een successfully
+00024760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024770: 2074 7261 6e73 6d69 7474 6564 2e0a 0a20   transmitted... 
+00024780: 2020 2020 2020 2020 2020 2070 726f 6772             progr
+00024790: 6573 735f 6172 6773 2028 6060 7475 706c  ess_args (``tupl
+000247a0: 6560 602c 202a 6f70 7469 6f6e 616c 2a29  e``, *optional*)
+000247b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000247c0: 2020 4578 7472 6120 6375 7374 6f6d 2061    Extra custom a
+000247d0: 7267 756d 656e 7473 2066 6f72 2074 6865  rguments for the
+000247e0: 2070 726f 6772 6573 7320 6361 6c6c 6261   progress callba
+000247f0: 636b 2066 756e 6374 696f 6e2e 0a20 2020  ck function..   
+00024800: 2020 2020 2020 2020 2020 2020 2059 6f75               You
+00024810: 2063 616e 2070 6173 7320 616e 7974 6869   can pass anythi
+00024820: 6e67 2079 6f75 206e 6565 6420 746f 2062  ng you need to b
+00024830: 6520 6176 6169 6c61 626c 6520 696e 2074  e available in t
+00024840: 6865 2070 726f 6772 6573 7320 6361 6c6c  he progress call
+00024850: 6261 636b 2073 636f 7065 3b20 666f 7220  back scope; for 
+00024860: 6578 616d 706c 652c 2061 204d 6573 7361  example, a Messa
+00024870: 6765 0a20 2020 2020 2020 2020 2020 2020  ge.             
+00024880: 2020 206f 626a 6563 7420 6f72 2061 2043     object or a C
+00024890: 6c69 656e 7420 696e 7374 616e 6365 2069  lient instance i
+000248a0: 6e20 6f72 6465 7220 746f 2065 6469 7420  n order to edit 
+000248b0: 7468 6520 6d65 7373 6167 6520 7769 7468  the message with
+000248c0: 2074 6865 2075 7064 6174 6564 2070 726f   the updated pro
+000248d0: 6772 6573 7320 7374 6174 7573 2e0a 0a20  gress status... 
+000248e0: 2020 2020 2020 204f 7468 6572 2050 6172         Other Par
+000248f0: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
+00024900: 2020 2020 2063 7572 7265 6e74 2028 6060       current (``
+00024910: 696e 7460 6029 3a0a 2020 2020 2020 2020  int``):.        
+00024920: 2020 2020 2020 2020 5468 6520 616d 6f75          The amou
+00024930: 6e74 206f 6620 6279 7465 7320 7472 616e  nt of bytes tran
+00024940: 736d 6974 7465 6420 736f 2066 6172 2e0a  smitted so far..
+00024950: 0a20 2020 2020 2020 2020 2020 2074 6f74  .            tot
+00024960: 616c 2028 6060 696e 7460 6029 3a0a 2020  al (``int``):.  
+00024970: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00024980: 6520 746f 7461 6c20 7369 7a65 206f 6620  e total size of 
+00024990: 7468 6520 6669 6c65 2e0a 0a20 2020 2020  the file...     
+000249a0: 2020 2020 2020 202a 6172 6773 2028 6060         *args (``
+000249b0: 7475 706c 6560 602c 202a 6f70 7469 6f6e  tuple``, *option
+000249c0: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
+000249d0: 2020 2020 2020 4578 7472 6120 6375 7374        Extra cust
+000249e0: 6f6d 2061 7267 756d 656e 7473 2061 7320  om arguments as 
+000249f0: 6465 6669 6e65 6420 696e 2074 6865 2060  defined in the `
+00024a00: 6070 726f 6772 6573 735f 6172 6773 6060  `progress_args``
+00024a10: 2070 6172 616d 6574 6572 2e0a 2020 2020   parameter..    
+00024a20: 2020 2020 2020 2020 2020 2020 596f 7520              You 
+00024a30: 6361 6e20 6569 7468 6572 206b 6565 7020  can either keep 
+00024a40: 6060 2a61 7267 7360 6020 6f72 2061 6464  ``*args`` or add
+00024a50: 2065 7665 7279 2073 696e 676c 6520 6578   every single ex
+00024a60: 7472 6120 6172 6775 6d65 6e74 2069 6e20  tra argument in 
+00024a70: 796f 7572 2066 756e 6374 696f 6e20 7369  your function si
+00024a80: 676e 6174 7572 652e 0a0a 2020 2020 2020  gnature...      
+00024a90: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00024aa0: 2020 2020 2020 204f 6e20 7375 6363 6573         On succes
+00024ab0: 732c 2074 6865 2061 6273 6f6c 7574 6520  s, the absolute 
+00024ac0: 7061 7468 206f 6620 7468 6520 646f 776e  path of the down
+00024ad0: 6c6f 6164 6564 2066 696c 6520 6173 2073  loaded file as s
+00024ae0: 7472 696e 6720 6973 2072 6574 7572 6e65  tring is returne
+00024af0: 642c 204e 6f6e 6520 6f74 6865 7277 6973  d, None otherwis
+00024b00: 652e 0a0a 2020 2020 2020 2020 5261 6973  e...        Rais
+00024b10: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00024b20: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
+00024b30: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
+00024b40: 5250 4320 6572 726f 722e 0a20 2020 2020  RPC error..     
+00024b50: 2020 2020 2020 2060 6056 616c 7565 4572         ``ValueEr
+00024b60: 726f 7260 603a 2049 6620 7468 6520 6d65  ror``: If the me
+00024b70: 7373 6167 6520 646f 6573 6e27 7420 636f  ssage doesn't co
+00024b80: 6e74 6169 6e20 616e 7920 646f 776e 6c6f  ntain any downlo
+00024b90: 6164 6162 6c65 206d 6564 6961 0a20 2020  adable media.   
+00024ba0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00024bb0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+00024bc0: 6c66 2e5f 636c 6965 6e74 2e64 6f77 6e6c  lf._client.downl
+00024bd0: 6f61 645f 6d65 6469 6128 0a20 2020 2020  oad_media(.     
+00024be0: 2020 2020 2020 206d 6573 7361 6765 3d73         message=s
+00024bf0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00024c00: 2066 696c 655f 6e61 6d65 3d66 696c 655f   file_name=file_
+00024c10: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00024c20: 2020 696e 5f6d 656d 6f72 793d 696e 5f6d    in_memory=in_m
+00024c30: 656d 6f72 792c 0a20 2020 2020 2020 2020  emory,.         
+00024c40: 2020 2062 6c6f 636b 3d62 6c6f 636b 2c0a     block=block,.
+00024c50: 2020 2020 2020 2020 2020 2020 7072 6f67              prog
+00024c60: 7265 7373 3d70 726f 6772 6573 732c 0a20  ress=progress,. 
+00024c70: 2020 2020 2020 2020 2020 2070 726f 6772             progr
+00024c80: 6573 735f 6172 6773 3d70 726f 6772 6573  ess_args=progres
+00024c90: 735f 6172 6773 2c0a 2020 2020 2020 2020  s_args,.        
+00024ca0: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+00024cb0: 2076 6f74 6528 0a20 2020 2020 2020 2073   vote(.        s
+00024cc0: 656c 662c 0a20 2020 2020 2020 206f 7074  elf,.        opt
+00024cd0: 696f 6e3a 2069 6e74 2c0a 2020 2020 2920  ion: int,.    ) 
+00024ce0: 2d3e 2022 7479 7065 732e 506f 6c6c 223a  -> "types.Poll":
+00024cf0: 0a20 2020 2020 2020 2022 2222 426f 756e  .        """Boun
+00024d00: 6420 6d65 7468 6f64 202a 766f 7465 2a20  d method *vote* 
+00024d10: 6f66 203a 6f62 6a3a 607e 7079 726f 6772  of :obj:`~pyrogr
+00024d20: 616d 2e74 7970 6573 2e4d 6573 7361 6765  am.types.Message
+00024d30: 602e 0a0a 2020 2020 2020 2020 5573 6520  `...        Use 
+00024d40: 6173 2061 2073 686f 7274 6375 7420 666f  as a shortcut fo
+00024d50: 723a 0a0a 2020 2020 2020 2020 2e2e 2063  r:..        .. c
+00024d60: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00024d70: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+00024d80: 636c 6965 6e74 2e76 6f74 655f 706f 6c6c  client.vote_poll
+00024d90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00024da0: 2020 6368 6174 5f69 643d 6d65 7373 6167    chat_id=messag
+00024db0: 652e 6368 6174 2e69 642c 0a20 2020 2020  e.chat.id,.     
+00024dc0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00024dd0: 6765 5f69 643d 6d65 7373 6167 652e 6964  ge_id=message.id
+00024de0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00024df0: 2020 6f70 7469 6f6e 3d31 0a20 2020 2020    option=1.     
+00024e00: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00024e10: 2020 4578 616d 706c 653a 0a20 2020 2020    Example:.     
+00024e20: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+00024e30: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+00024e40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00024e50: 6573 7361 6765 2e76 6f74 6528 3629 0a0a  essage.vote(6)..
+00024e60: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00024e70: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00024e80: 6f70 7469 6f6e 2028 6060 696e 7460 6029  option (``int``)
+00024e90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00024ea0: 2020 496e 6465 7820 6f66 2074 6865 2070    Index of the p
+00024eb0: 6f6c 6c20 6f70 7469 6f6e 2079 6f75 2077  oll option you w
+00024ec0: 616e 7420 746f 2076 6f74 6520 666f 7220  ant to vote for 
+00024ed0: 2830 2074 6f20 3929 2e0a 0a20 2020 2020  (0 to 9)...     
+00024ee0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00024ef0: 2020 2020 2020 2020 3a6f 626a 3a60 7e70          :obj:`~p
+00024f00: 7972 6f67 7261 6d2e 7479 7065 732e 506f  yrogram.types.Po
+00024f10: 6c6c 603a 204f 6e20 7375 6363 6573 732c  ll`: On success,
+00024f20: 2074 6865 2070 6f6c 6c20 7769 7468 2074   the poll with t
+00024f30: 6865 2063 686f 7365 6e20 6f70 7469 6f6e  he chosen option
+00024f40: 2069 7320 7265 7475 726e 6564 2e0a 0a20   is returned... 
+00024f50: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
+00024f60: 2020 2020 2020 2020 2020 2052 5043 4572             RPCEr
+00024f70: 726f 723a 2049 6e20 6361 7365 206f 6620  ror: In case of 
+00024f80: 6120 5465 6c65 6772 616d 2052 5043 2065  a Telegram RPC e
+00024f90: 7272 6f72 2e0a 2020 2020 2020 2020 2222  rror..        ""
+00024fa0: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+00024fb0: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
+00024fc0: 6965 6e74 2e76 6f74 655f 706f 6c6c 280a  ient.vote_poll(.
+00024fd0: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+00024fe0: 5f69 643d 7365 6c66 2e63 6861 742e 6964  _id=self.chat.id
+00024ff0: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
+00025000: 7373 6167 655f 6964 3d73 656c 662e 6964  ssage_id=self.id
+00025010: 2c0a 2020 2020 2020 2020 2020 2020 6f70  ,.            op
+00025020: 7469 6f6e 733d 6f70 7469 6f6e 0a20 2020  tions=option.   
+00025030: 2020 2020 2029 0a0a 2020 2020 6173 796e       )..    asyn
+00025040: 6320 6465 6620 7069 6e28 7365 6c66 2c20  c def pin(self, 
+00025050: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00025060: 7469 6f6e 3a20 626f 6f6c 203d 2046 616c  tion: bool = Fal
+00025070: 7365 2c20 626f 7468 5f73 6964 6573 3a20  se, both_sides: 
+00025080: 626f 6f6c 203d 2046 616c 7365 2920 2d3e  bool = False) ->
+00025090: 2022 7479 7065 732e 4d65 7373 6167 6522   "types.Message"
+000250a0: 3a0a 2020 2020 2020 2020 2222 2242 6f75  :.        """Bou
+000250b0: 6e64 206d 6574 686f 6420 2a70 696e 2a20  nd method *pin* 
+000250c0: 6f66 203a 6f62 6a3a 607e 7079 726f 6772  of :obj:`~pyrogr
+000250d0: 616d 2e74 7970 6573 2e4d 6573 7361 6765  am.types.Message
+000250e0: 602e 0a0a 2020 2020 2020 2020 5573 6520  `...        Use 
+000250f0: 6173 2061 2073 686f 7274 6375 7420 666f  as a shortcut fo
+00025100: 723a 0a0a 2020 2020 2020 2020 2e2e 2063  r:..        .. c
+00025110: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00025120: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+00025130: 6177 6169 7420 636c 6965 6e74 2e70 696e  await client.pin
+00025140: 5f63 6861 745f 6d65 7373 6167 6528 0a20  _chat_message(. 
+00025150: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00025160: 6861 745f 6964 3d6d 6573 7361 6765 2e63  hat_id=message.c
+00025170: 6861 742e 6964 2c0a 2020 2020 2020 2020  hat.id,.        
+00025180: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+00025190: 6964 3d6d 6573 7361 6765 5f69 640a 2020  id=message_id.  
+000251a0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000251b0: 2020 2020 2045 7861 6d70 6c65 3a0a 2020       Example:.  
+000251c0: 2020 2020 2020 2020 2020 2e2e 2063 6f64            .. cod
+000251d0: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+000251e0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000251f0: 2020 6177 6169 7420 6d65 7373 6167 652e    await message.
+00025200: 7069 6e28 290a 0a20 2020 2020 2020 2050  pin()..        P
+00025210: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
+00025220: 2020 2020 2020 2064 6973 6162 6c65 5f6e         disable_n
+00025230: 6f74 6966 6963 6174 696f 6e20 2860 6062  otification (``b
+00025240: 6f6f 6c60 6029 3a0a 2020 2020 2020 2020  ool``):.        
+00025250: 2020 2020 2020 2020 5061 7373 2054 7275          Pass Tru
+00025260: 652c 2069 6620 6974 2069 7320 6e6f 7420  e, if it is not 
+00025270: 6e65 6365 7373 6172 7920 746f 2073 656e  necessary to sen
+00025280: 6420 6120 6e6f 7469 6669 6361 7469 6f6e  d a notification
+00025290: 2074 6f20 616c 6c20 6368 6174 206d 656d   to all chat mem
+000252a0: 6265 7273 2061 626f 7574 2074 6865 206e  bers about the n
+000252b0: 6577 2070 696e 6e65 640a 2020 2020 2020  ew pinned.      
+000252c0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+000252d0: 652e 204e 6f74 6966 6963 6174 696f 6e73  e. Notifications
+000252e0: 2061 7265 2061 6c77 6179 7320 6469 7361   are always disa
+000252f0: 626c 6564 2069 6e20 6368 616e 6e65 6c73  bled in channels
+00025300: 2e0a 0a20 2020 2020 2020 2020 2020 2062  ...            b
+00025310: 6f74 685f 7369 6465 7320 2860 6062 6f6f  oth_sides (``boo
+00025320: 6c60 602c 202a 6f70 7469 6f6e 616c 2a29  l``, *optional*)
+00025330: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00025340: 2020 5061 7373 2054 7275 6520 746f 2070    Pass True to p
+00025350: 696e 2074 6865 206d 6573 7361 6765 2066  in the message f
+00025360: 6f72 2062 6f74 6820 7369 6465 7320 2879  or both sides (y
+00025370: 6f75 2061 6e64 2072 6563 6970 6965 6e74  ou and recipient
+00025380: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
+00025390: 2020 2041 7070 6c69 6361 626c 6520 746f     Applicable to
+000253a0: 2070 7269 7661 7465 2063 6861 7473 206f   private chats o
+000253b0: 6e6c 792e 2044 6566 6175 6c74 7320 746f  nly. Defaults to
+000253c0: 2046 616c 7365 2e0a 0a20 2020 2020 2020   False...       
+000253d0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+000253e0: 2020 2020 2020 3a6f 626a 3a60 7e70 7972        :obj:`~pyr
+000253f0: 6f67 7261 6d2e 7479 7065 732e 4d65 7373  ogram.types.Mess
+00025400: 6167 6560 3a20 4f6e 2073 7563 6365 7373  age`: On success
+00025410: 2c20 7468 6520 7365 7276 6963 6520 6d65  , the service me
+00025420: 7373 6167 6520 6973 2072 6574 7572 6e65  ssage is returne
+00025430: 642e 0a0a 2020 2020 2020 2020 5261 6973  d...        Rais
+00025440: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00025450: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
+00025460: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
+00025470: 5250 4320 6572 726f 722e 0a20 2020 2020  RPC error..     
+00025480: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00025490: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+000254a0: 2e5f 636c 6965 6e74 2e70 696e 5f63 6861  ._client.pin_cha
+000254b0: 745f 6d65 7373 6167 6528 0a20 2020 2020  t_message(.     
+000254c0: 2020 2020 2020 2063 6861 745f 6964 3d73         chat_id=s
+000254d0: 656c 662e 6368 6174 2e69 642c 0a20 2020  elf.chat.id,.   
+000254e0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+000254f0: 5f69 643d 7365 6c66 2e69 642c 0a20 2020  _id=self.id,.   
+00025500: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
+00025510: 5f6e 6f74 6966 6963 6174 696f 6e3d 6469  _notification=di
+00025520: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+00025530: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00025540: 626f 7468 5f73 6964 6573 3d62 6f74 685f  both_sides=both_
+00025550: 7369 6465 730a 2020 2020 2020 2020 290a  sides.        ).
+00025560: 0a20 2020 2061 7379 6e63 2064 6566 2075  .    async def u
+00025570: 6e70 696e 2873 656c 6629 202d 3e20 626f  npin(self) -> bo
+00025580: 6f6c 3a0a 2020 2020 2020 2020 2222 2242  ol:.        """B
+00025590: 6f75 6e64 206d 6574 686f 6420 2a75 6e70  ound method *unp
+000255a0: 696e 2a20 6f66 203a 6f62 6a3a 607e 7079  in* of :obj:`~py
+000255b0: 726f 6772 616d 2e74 7970 6573 2e4d 6573  rogram.types.Mes
+000255c0: 7361 6765 602e 0a0a 2020 2020 2020 2020  sage`...        
+000255d0: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
+000255e0: 7420 666f 723a 0a0a 2020 2020 2020 2020  t for:..        
+000255f0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+00025600: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+00025610: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
+00025620: 2e75 6e70 696e 5f63 6861 745f 6d65 7373  .unpin_chat_mess
+00025630: 6167 6528 0a20 2020 2020 2020 2020 2020  age(.           
+00025640: 2020 2020 2063 6861 745f 6964 3d6d 6573       chat_id=mes
+00025650: 7361 6765 2e63 6861 742e 6964 2c0a 2020  sage.chat.id,.  
+00025660: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00025670: 7373 6167 655f 6964 3d6d 6573 7361 6765  ssage_id=message
+00025680: 5f69 640a 2020 2020 2020 2020 2020 2020  _id.            
+00025690: 290a 0a20 2020 2020 2020 2045 7861 6d70  )..        Examp
+000256a0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+000256b0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+000256c0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+000256d0: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
+000256e0: 7373 6167 652e 756e 7069 6e28 290a 0a20  ssage.unpin().. 
+000256f0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00025700: 2020 2020 2020 2020 2020 2020 5472 7565              True
+00025710: 206f 6e20 7375 6363 6573 732e 0a0a 2020   on success...  
+00025720: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+00025730: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
+00025740: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
+00025750: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
+00025760: 726f 722e 0a20 2020 2020 2020 2022 2222  ror..        """
+00025770: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00025780: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
+00025790: 6e74 2e75 6e70 696e 5f63 6861 745f 6d65  nt.unpin_chat_me
+000257a0: 7373 6167 6528 0a20 2020 2020 2020 2020  ssage(.         
+000257b0: 2020 2063 6861 745f 6964 3d73 656c 662e     chat_id=self.
+000257c0: 6368 6174 2e69 642c 0a20 2020 2020 2020  chat.id,.       
+000257d0: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
+000257e0: 7365 6c66 2e69 640a 2020 2020 2020 2020  self.id.        
+000257f0: 290a                                     ).
```

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/message_entity.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/message_reactions.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/photo.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/poll.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/poll_option.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/reaction.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/sticker.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/stickerset.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/stickerset.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/thumbnail.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/venue.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/video.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/video_note.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/voice.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/web_app_data.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/messages_and_media/web_page.py` & `PyroFork-2.2.0/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/object.py` & `PyroFork-2.2.0/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/update.py` & `PyroFork-2.2.0/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/__init__.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_event.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_event_filter.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_invite_link.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_join_request.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_joiner.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_member.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_member_updated.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_permissions.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_photo.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_preview.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_privileges.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/chat_reactions.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/dialog.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/emoji_status.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/forum_topic.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/forum_topic_closed.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/forum_topic_created.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/forum_topic_edited.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/invite_link_importer.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/peer_channel.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/peer_user.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/peer_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/restriction.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/user.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/username.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/video_chat_ended.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/types/user_and_chats/video_chat_started.py` & `PyroFork-2.2.0/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/pyrogram/utils.py` & `PyroFork-2.2.0/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/setup.py` & `PyroFork-2.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,16 +53,14 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet",
@@ -74,15 +72,15 @@
     ],
     keywords="telegram chat messenger mtproto api client library python",
     project_urls={
         "Tracker": "https://github.com/Mayuri-Chan/pyrofork/issues",
         "Source": "https://github.com/Mayuri-Chan/pyrofork",
         "Documentation": "https://pyrofork.mayuri.my.id",
     },
-    python_requires="~=3.7",
+    python_requires="~=3.9",
     package_data={
         "pyrogram": ["py.typed"],
     },
     packages=find_packages(exclude=["compiler*", "tests*"]),
     zip_safe=False,
     install_requires=requires
 )
```

### Comparing `PyroFork-2.1.8/tests/__init__.py` & `PyroFork-2.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/tests/filters/__init__.py` & `PyroFork-2.2.0/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/tests/filters/test_command.py` & `PyroFork-2.2.0/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/tests/parser/__init__.py` & `PyroFork-2.2.0/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/tests/parser/test_html.py` & `PyroFork-2.2.0/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.8/tests/test_file_id.py` & `PyroFork-2.2.0/tests/test_file_id.py`

 * *Files identical despite different names*

