# Comparing `tmp/chitose-0.0.5.tar.gz` & `tmp/chitose-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "chitose-0.0.6.tar", max compression
```

## Comparing `chitose-0.0.5.tar` & `chitose-0.0.6.tar`

### file list

```diff
@@ -1,170 +1,143 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 chitose-0.0.5/.gitmodules
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 chitose-0.0.5/.readthedocs.yaml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/__init__.py
--rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/agent.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/blob.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/link.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/object.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/record.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/xrpc.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/__init__.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/get_preferences.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/put_preferences.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/defs.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/post.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/repost.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/block.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/defs.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/follow.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_list.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_list_mutes.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_lists.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/list.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/listitem.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/mute_actor_list.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/unmute_actor_list.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/__init__.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0    12486 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/disable_account_invites.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/enable_account_invites.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/label/defs.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/rebase_repo.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/create_account.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/defs.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/make.bat
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.actor.rst
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.embed.rst
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.feed.rst
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.graph.rst
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.notification.rst
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.richtext.rst
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.rst
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.unspecced.rst
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.rst
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.admin.rst
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.identity.rst
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.label.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.moderation.rst
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.repo.rst
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.rst
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.server.rst
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.sync.rst
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.rst
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.rst
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/conf.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/index.rst
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/modules.rst
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/get_profiles.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/get_timeline.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/post.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/post_with_image.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/quote_post.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/simple_get_timeline.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/simple_post.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chitose-0.0.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 chitose-0.0.5/LICENSE
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 chitose-0.0.5/README.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 chitose-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 chitose-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-21 03:09:41.620752 chitose-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3483 2023-05-21 03:09:41.620752 chitose-0.0.6/README.md
+-rw-r--r--   0        0        0      221 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/__init__.py
+-rw-r--r--   0        0        0     7877 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/agent.py
+-rw-r--r--   0        0        0      478 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/__init__.py
+-rw-r--r--   0        0        0     1207 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/__init__.py
+-rw-r--r--   0        0        0     2198 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     5314 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      314 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/get_preferences.py
+-rw-r--r--   0        0        0      286 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      297 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      453 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      682 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      466 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/put_preferences.py
+-rw-r--r--   0        0        0      467 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      435 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      372 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1717 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1343 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2511 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1145 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0     3748 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     6930 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0     1037 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/describe_feed_generator.py
+-rw-r--r--   0        0        0      926 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/generator.py
+-rw-r--r--   0        0        0      462 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_actor_feeds.py
+-rw-r--r--   0        0        0      439 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0      461 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_feed.py
+-rw-r--r--   0        0        0      387 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_feed_generator.py
+-rw-r--r--   0        0        0      353 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_feed_generators.py
+-rw-r--r--   0        0        0      463 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_feed_skeleton.py
+-rw-r--r--   0        0        0      902 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      352 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      310 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0      453 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      477 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      480 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2470 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      484 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0     3094 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      398 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/block.py
+-rw-r--r--   0        0        0     2637 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/defs.py
+-rw-r--r--   0        0        0      400 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      415 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0      437 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0      433 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      420 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_list.py
+-rw-r--r--   0        0        0      428 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_list_mutes.py
+-rw-r--r--   0        0        0      448 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_lists.py
+-rw-r--r--   0        0        0      398 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0      969 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/list.py
+-rw-r--r--   0        0        0      459 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/listitem.py
+-rw-r--r--   0        0        0      345 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      342 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/mute_actor_list.py
+-rw-r--r--   0        0        0      351 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      348 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/graph/unmute_actor_list.py
+-rw-r--r--   0        0        0     1200 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1641 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      379 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      375 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1327 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      719 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      497 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      373 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/blob.py
+-rw-r--r--   0        0        0      490 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/__init__.py
+-rw-r--r--   0        0        0     1186 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/__init__.py
+-rw-r--r--   0        0        0     5949 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0    13162 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      438 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/disable_account_invites.py
+-rw-r--r--   0        0        0      516 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      399 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/enable_account_invites.py
+-rw-r--r--   0        0        0      494 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      338 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      504 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      338 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0      785 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      369 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      309 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      489 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      438 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0      538 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1061 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      478 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      414 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      935 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      466 2023-05-21 03:09:41.620752 chitose-0.0.6/chitose/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      362 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0     1030 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1096 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/label/defs.py
+-rw-r--r--   0        0        0      810 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0      820 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      931 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0      735 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      740 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0     5687 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     1929 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0      923 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      884 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0      410 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0      693 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1418 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1066 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      568 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/rebase_repo.py
+-rw-r--r--   0        0        0      392 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      355 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0     4551 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0      607 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      767 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      447 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0      827 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0      521 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1191 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      433 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      293 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0      782 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      496 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      304 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      634 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      302 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      324 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      390 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      407 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      372 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0     4350 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      430 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      387 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      500 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      591 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      356 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      574 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      618 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      593 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0      686 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      530 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      440 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2945 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      170 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/link.py
+-rw-r--r--   0        0        0      136 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/object.py
+-rw-r--r--   0        0        0      136 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/record.py
+-rw-r--r--   0        0        0     1379 2023-05-21 03:09:41.624752 chitose-0.0.6/chitose/xrpc.py
+-rw-r--r--   0        0        0      801 2023-05-21 03:09:41.624752 chitose-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4286 1970-01-01 00:00:00.000000 chitose-0.0.6/PKG-INFO
```

### Comparing `chitose-0.0.5/chitose/agent.py` & `chitose-0.0.6/chitose/agent.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/xrpc.py` & `chitose-0.0.6/chitose/xrpc.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/__init__.py` & `chitose-0.0.6/chitose/app/bsky/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/actor/__init__.py` & `chitose-0.0.6/chitose/app/bsky/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/actor/defs.py` & `chitose-0.0.6/chitose/app/bsky/actor/defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,37 +56,47 @@
 
     def to_dict(self) -> dict:
         return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'banner': self.banner, 'followersCount': self.followers_count, 'followsCount': self.follows_count, 'postsCount': self.posts_count, 'indexedAt': self.indexed_at, 'viewer': self.viewer, 'labels': self.labels, '$type': 'app.bsky.actor.defs#profileViewDetailed'}
 
 class ViewerState(chitose.Object):
     """"""
 
-    def __init__(self, muted: typing.Optional[str]=None, muted_by_list: typing.Optional[chitose.app.bsky.graph.defs.ListViewBasic]=None, blocked_by: typing.Optional[str]=None, blocking: typing.Optional[str]=None, following: typing.Optional[str]=None, followed_by: typing.Optional[str]=None) -> None:
+    def __init__(self, muted: typing.Optional[bool]=None, muted_by_list: typing.Optional[chitose.app.bsky.graph.defs.ListViewBasic]=None, blocked_by: typing.Optional[bool]=None, blocking: typing.Optional[str]=None, following: typing.Optional[str]=None, followed_by: typing.Optional[str]=None) -> None:
         self.muted = muted
         self.muted_by_list = muted_by_list
         self.blocked_by = blocked_by
         self.blocking = blocking
         self.following = following
         self.followed_by = followed_by
 
     def to_dict(self) -> dict:
         return {'muted': self.muted, 'mutedByList': self.muted_by_list, 'blockedBy': self.blocked_by, 'blocking': self.blocking, 'following': self.following, 'followedBy': self.followed_by, '$type': 'app.bsky.actor.defs#viewerState'}
-Preferences = list[typing.Union['chitose.app.bsky.actor.defs.AdultContentPref', 'chitose.app.bsky.actor.defs.ContentLabelPref']]
+Preferences = list[typing.Union['chitose.app.bsky.actor.defs.AdultContentPref', 'chitose.app.bsky.actor.defs.ContentLabelPref', 'chitose.app.bsky.actor.defs.SavedFeedsPref']]
 
 class AdultContentPref(chitose.Object):
     """"""
 
-    def __init__(self, enabled: str) -> None:
+    def __init__(self, enabled: bool) -> None:
         self.enabled = enabled
 
     def to_dict(self) -> dict:
         return {'enabled': self.enabled, '$type': 'app.bsky.actor.defs#adultContentPref'}
 
 class ContentLabelPref(chitose.Object):
     """"""
 
     def __init__(self, label: str, visibility: typing.Literal['show', 'warn', 'hide']) -> None:
         self.label = label
         self.visibility = visibility
 
     def to_dict(self) -> dict:
-        return {'label': self.label, 'visibility': self.visibility, '$type': 'app.bsky.actor.defs#contentLabelPref'}
+        return {'label': self.label, 'visibility': self.visibility, '$type': 'app.bsky.actor.defs#contentLabelPref'}
+
+class SavedFeedsPref(chitose.Object):
+    """"""
+
+    def __init__(self, pinned: list[str], saved: list[str]) -> None:
+        self.pinned = pinned
+        self.saved = saved
+
+    def to_dict(self) -> dict:
+        return {'pinned': self.pinned, 'saved': self.saved, '$type': 'app.bsky.actor.defs#savedFeedsPref'}
```

### Comparing `chitose-0.0.5/chitose/app/bsky/actor/profile.py` & `chitose-0.0.6/chitose/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/embed/external.py` & `chitose-0.0.6/chitose/app/bsky/embed/external.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/embed/images.py` & `chitose-0.0.6/chitose/app/bsky/embed/images.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/embed/record.py` & `chitose-0.0.6/chitose/app/bsky/embed/record.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import chitose.app.bsky.embed.external
 import chitose.app.bsky.embed.images
 import chitose.app.bsky.embed.record
 import chitose.app.bsky.embed.record_with_media
+import chitose.app.bsky.feed.defs
 import chitose.com.atproto.label.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
 class Record(chitose.Object):
     """"""
 
@@ -19,15 +20,15 @@
 
     def to_dict(self) -> dict:
         return {'record': self.record, '$type': 'app.bsky.embed.record'}
 
 class View(chitose.Object):
     """"""
 
-    def __init__(self, record: typing.Union[chitose.app.bsky.embed.record.ViewRecord, chitose.app.bsky.embed.record.ViewNotFound, chitose.app.bsky.embed.record.ViewBlocked]) -> None:
+    def __init__(self, record: typing.Union[chitose.app.bsky.embed.record.ViewRecord, chitose.app.bsky.embed.record.ViewNotFound, chitose.app.bsky.embed.record.ViewBlocked, chitose.app.bsky.feed.defs.GeneratorView]) -> None:
         self.record = record
 
     def to_dict(self) -> dict:
         return {'record': self.record, '$type': 'app.bsky.embed.record#view'}
 
 class ViewRecord(chitose.Object):
     """"""
```

### Comparing `chitose-0.0.5/chitose/app/bsky/embed/record_with_media.py` & `chitose-0.0.6/chitose/app/bsky/embed/record_with_media.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/feed/__init__.py` & `chitose-0.0.6/chitose/app/bsky/feed/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
+from .describe_feed_generator import _describe_feed_generator
+from .get_actor_feeds import _get_actor_feeds
 from .get_author_feed import _get_author_feed
+from .get_feed import _get_feed
+from .get_feed_generator import _get_feed_generator
+from .get_feed_generators import _get_feed_generators
+from .get_feed_skeleton import _get_feed_skeleton
 from .get_likes import _get_likes
 from .get_post_thread import _get_post_thread
 from .get_posts import _get_posts
 from .get_reposted_by import _get_reposted_by
 from .get_timeline import _get_timeline
 import chitose.app.bsky.actor.defs
 import typing
@@ -12,18 +18,26 @@
 class Feed_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
+    def get_feed_generators(self, feeds: list[str]) -> bytes:
+        """Get information about a list of feed generators"""
+        return _get_feed_generators(self.service, self.headers, feeds)
+
     def get_timeline(self, algorithm: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """A view of the user's home timeline."""
         return _get_timeline(self.service, self.headers, algorithm, limit, cursor)
 
+    def get_feed_generator(self, feed: str) -> bytes:
+        """Get information about a specific feed offered by a feed generator, such as its online status"""
+        return _get_feed_generator(self.service, self.headers, feed)
+
     def get_author_feed(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """A view of an actor's feed."""
         return _get_author_feed(self.service, self.headers, actor, limit, cursor)
 
     def get_likes(self, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """"""
         return _get_likes(self.service, self.headers, uri, cid, limit, cursor)
@@ -32,10 +46,26 @@
         """"""
         return _get_post_thread(self.service, self.headers, uri, depth)
 
     def get_reposted_by(self, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """"""
         return _get_reposted_by(self.service, self.headers, uri, cid, limit, cursor)
 
+    def describe_feed_generator(self) -> bytes:
+        """Returns information about a given feed generator including TOS & offered feed URIs"""
+        return _describe_feed_generator(self.service, self.headers)
+
     def get_posts(self, uris: list[str]) -> bytes:
         """A view of an actor's feed."""
-        return _get_posts(self.service, self.headers, uris)
+        return _get_posts(self.service, self.headers, uris)
+
+    def get_feed(self, feed: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+        """Compose and hydrate a feed from a user's selected feed generator"""
+        return _get_feed(self.service, self.headers, feed, limit, cursor)
+
+    def get_feed_skeleton(self, feed: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+        """A skeleton of a feed provided by a feed generator"""
+        return _get_feed_skeleton(self.service, self.headers, feed, limit, cursor)
+
+    def get_actor_feeds(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+        """Retrieve a list of feeds created by a given actor"""
+        return _get_actor_feeds(self.service, self.headers, actor, limit, cursor)
```

### Comparing `chitose-0.0.5/chitose/app/bsky/feed/defs.py` & `chitose-0.0.6/chitose/app/bsky/feed/defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import chitose
 import chitose.app.bsky.actor.defs
 import chitose.app.bsky.embed.external
 import chitose.app.bsky.embed.images
 import chitose.app.bsky.embed.record
 import chitose.app.bsky.embed.record_with_media
 import chitose.app.bsky.feed.defs
+import chitose.app.bsky.richtext.facet
 import chitose.com.atproto.label.defs
 import typing
 
 class PostView(chitose.Object):
     """"""
 
     def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileViewBasic, record: typing.Any, indexed_at: str, embed: typing.Optional[typing.Union[chitose.app.bsky.embed.images.View, chitose.app.bsky.embed.external.View, chitose.app.bsky.embed.record.View, chitose.app.bsky.embed.record_with_media.View]]=None, reply_count: typing.Optional[int]=None, repost_count: typing.Optional[int]=None, like_count: typing.Optional[int]=None, viewer: typing.Optional[chitose.app.bsky.feed.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
@@ -50,15 +51,15 @@
 
     def to_dict(self) -> dict:
         return {'post': self.post, 'reply': self.reply, 'reason': self.reason, '$type': 'app.bsky.feed.defs#feedViewPost'}
 
 class ReplyRef(chitose.Object):
     """"""
 
-    def __init__(self, root: chitose.app.bsky.feed.defs.PostView, parent: chitose.app.bsky.feed.defs.PostView) -> None:
+    def __init__(self, root: typing.Union[chitose.app.bsky.feed.defs.PostView, chitose.app.bsky.feed.defs.NotFoundPost, chitose.app.bsky.feed.defs.BlockedPost], parent: typing.Union[chitose.app.bsky.feed.defs.PostView, chitose.app.bsky.feed.defs.NotFoundPost, chitose.app.bsky.feed.defs.BlockedPost]) -> None:
         self.root = root
         self.parent = parent
 
     def to_dict(self) -> dict:
         return {'root': self.root, 'parent': self.parent, '$type': 'app.bsky.feed.defs#replyRef'}
 
 class ReasonRepost(chitose.Object):
@@ -81,23 +82,70 @@
 
     def to_dict(self) -> dict:
         return {'post': self.post, 'parent': self.parent, 'replies': self.replies, '$type': 'app.bsky.feed.defs#threadViewPost'}
 
 class NotFoundPost(chitose.Object):
     """"""
 
-    def __init__(self, uri: str, not_found: str) -> None:
+    def __init__(self, uri: str, not_found: bool) -> None:
         self.uri = uri
         self.not_found = not_found
 
     def to_dict(self) -> dict:
         return {'uri': self.uri, 'notFound': self.not_found, '$type': 'app.bsky.feed.defs#notFoundPost'}
 
 class BlockedPost(chitose.Object):
     """"""
 
-    def __init__(self, uri: str, blocked: str) -> None:
+    def __init__(self, uri: str, blocked: bool) -> None:
         self.uri = uri
         self.blocked = blocked
 
     def to_dict(self) -> dict:
-        return {'uri': self.uri, 'blocked': self.blocked, '$type': 'app.bsky.feed.defs#blockedPost'}
+        return {'uri': self.uri, 'blocked': self.blocked, '$type': 'app.bsky.feed.defs#blockedPost'}
+
+class GeneratorView(chitose.Object):
+    """"""
+
+    def __init__(self, uri: str, cid: str, creator: chitose.app.bsky.actor.defs.ProfileView, display_name: str, indexed_at: str, did: typing.Optional[str]=None, description: typing.Optional[str]=None, description_facets: typing.Optional[list[chitose.app.bsky.richtext.facet.Facet]]=None, avatar: typing.Optional[str]=None, like_count: typing.Optional[int]=None, viewer: typing.Optional[chitose.app.bsky.feed.defs.GeneratorViewerState]=None) -> None:
+        self.uri = uri
+        self.cid = cid
+        self.creator = creator
+        self.display_name = display_name
+        self.indexed_at = indexed_at
+        self.did = did
+        self.description = description
+        self.description_facets = description_facets
+        self.avatar = avatar
+        self.like_count = like_count
+        self.viewer = viewer
+
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'cid': self.cid, 'creator': self.creator, 'displayName': self.display_name, 'indexedAt': self.indexed_at, 'did': self.did, 'description': self.description, 'descriptionFacets': self.description_facets, 'avatar': self.avatar, 'likeCount': self.like_count, 'viewer': self.viewer, '$type': 'app.bsky.feed.defs#generatorView'}
+
+class GeneratorViewerState(chitose.Object):
+    """"""
+
+    def __init__(self, like: typing.Optional[str]=None) -> None:
+        self.like = like
+
+    def to_dict(self) -> dict:
+        return {'like': self.like, '$type': 'app.bsky.feed.defs#generatorViewerState'}
+
+class SkeletonFeedPost(chitose.Object):
+    """"""
+
+    def __init__(self, post: str, reason: typing.Optional[chitose.app.bsky.feed.defs.SkeletonReasonRepost]=None) -> None:
+        self.post = post
+        self.reason = reason
+
+    def to_dict(self) -> dict:
+        return {'post': self.post, 'reason': self.reason, '$type': 'app.bsky.feed.defs#skeletonFeedPost'}
+
+class SkeletonReasonRepost(chitose.Object):
+    """"""
+
+    def __init__(self, repost: str) -> None:
+        self.repost = repost
+
+    def to_dict(self) -> dict:
+        return {'repost': self.repost, '$type': 'app.bsky.feed.defs#skeletonReasonRepost'}
```

### Comparing `chitose-0.0.5/chitose/app/bsky/feed/get_likes.py` & `chitose-0.0.6/chitose/app/bsky/feed/get_likes.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/feed/post.py` & `chitose-0.0.6/chitose/app/bsky/feed/post.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/graph/__init__.py` & `chitose-0.0.6/chitose/app/bsky/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/graph/defs.py` & `chitose-0.0.6/chitose/app/bsky/graph/defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,12 +48,12 @@
         return {'subject': self.subject, '$type': 'app.bsky.graph.defs#listItemView'}
 ListPurpose = typing.Literal['app.bsky.graph.defs#modlist',]
 MODLIST = 'app.bsky.graph.defs#modlist'
 
 class ListViewerState(chitose.Object):
     """"""
 
-    def __init__(self, muted: typing.Optional[str]=None) -> None:
+    def __init__(self, muted: typing.Optional[bool]=None) -> None:
         self.muted = muted
 
     def to_dict(self) -> dict:
         return {'muted': self.muted, '$type': 'app.bsky.graph.defs#listViewerState'}
```

### Comparing `chitose-0.0.5/chitose/app/bsky/graph/list.py` & `chitose-0.0.6/chitose/app/bsky/graph/list.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/notification/__init__.py` & `chitose-0.0.6/chitose/app/bsky/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/notification/list_notifications.py` & `chitose-0.0.6/chitose/app/bsky/notification/list_notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class Notification(chitose.Object):
     """
 
 
     :param reason: Expected values are 'like', 'repost', 'follow', 'mention', 'reply', and 'quote'.
     """
 
-    def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileView, reason: typing.Literal['like', 'repost', 'follow', 'mention', 'reply', 'quote'], record: typing.Any, is_read: str, indexed_at: str, reason_subject: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
+    def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileView, reason: typing.Literal['like', 'repost', 'follow', 'mention', 'reply', 'quote'], record: typing.Any, is_read: bool, indexed_at: str, reason_subject: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.uri = uri
         self.cid = cid
         self.author = author
         self.reason = reason
         self.record = record
         self.is_read = is_read
         self.indexed_at = indexed_at
```

### Comparing `chitose-0.0.5/chitose/app/bsky/richtext/facet.py` & `chitose-0.0.6/chitose/app/bsky/richtext/facet.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/app/bsky/unspecced/__init__.py` & `chitose-0.0.6/chitose/app/bsky/unspecced/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 class Unspecced_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def get_popular(self, include_nsfw: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+    def get_popular(self, include_nsfw: typing.Optional[bool]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """An unspecced view of globally popular items"""
         return _get_popular(self.service, self.headers, include_nsfw, limit, cursor)
```

### Comparing `chitose-0.0.5/chitose/com/atproto/__init__.py` & `chitose-0.0.6/chitose/com/atproto/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/admin/__init__.py` & `chitose-0.0.6/chitose/com/atproto/admin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.service = service
         self.headers = headers
 
     def get_repo(self, did: str) -> bytes:
         """View details about a repository."""
         return _get_repo(self.service, self.headers, did)
 
-    def get_moderation_reports(self, subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+    def get_moderation_reports(self, subject: typing.Optional[str]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """List moderation reports related to a subject."""
         return _get_moderation_reports(self.service, self.headers, subject, resolved, action_type, limit, cursor)
 
     def take_moderation_action(self, action: typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge'], subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
         """Take a moderation action on a repo."""
         return _take_moderation_action(self.service, self.headers, action, subject, reason, created_by, subject_blob_cids, create_label_vals, negate_label_vals)
```

### Comparing `chitose-0.0.5/chitose/com/atproto/admin/defs.py` & `chitose-0.0.6/chitose/com/atproto/admin/defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def to_dict(self) -> dict:
         return {'id': self.id, 'action': self.action, 'subject': self.subject, 'subjectBlobCids': self.subject_blob_cids, 'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, 'resolvedReportIds': self.resolved_report_ids, 'createLabelVals': self.create_label_vals, 'negateLabelVals': self.negate_label_vals, 'reversal': self.reversal, '$type': 'com.atproto.admin.defs#actionView'}
 
 class ActionViewDetail(chitose.Object):
     """"""
 
-    def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoView, chitose.com.atproto.admin.defs.RecordView], subject_blobs: list[chitose.com.atproto.admin.defs.BlobView], reason: str, created_by: str, created_at: str, resolved_reports: list[chitose.com.atproto.admin.defs.ReportView], create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None, reversal: typing.Optional[chitose.com.atproto.admin.defs.ActionReversal]=None) -> None:
+    def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoView, chitose.com.atproto.admin.defs.RepoViewNotFound, chitose.com.atproto.admin.defs.RecordView, chitose.com.atproto.admin.defs.RecordViewNotFound], subject_blobs: list[chitose.com.atproto.admin.defs.BlobView], reason: str, created_by: str, created_at: str, resolved_reports: list[chitose.com.atproto.admin.defs.ReportView], create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None, reversal: typing.Optional[chitose.com.atproto.admin.defs.ActionReversal]=None) -> None:
         self.id = id
         self.action = action
         self.subject = subject
         self.subject_blobs = subject_blobs
         self.reason = reason
         self.created_by = created_by
         self.created_at = created_at
@@ -87,30 +87,30 @@
 
     def to_dict(self) -> dict:
         return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActionIds': self.resolved_by_action_ids, 'reason': self.reason, '$type': 'com.atproto.admin.defs#reportView'}
 
 class ReportViewDetail(chitose.Object):
     """"""
 
-    def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoView, chitose.com.atproto.admin.defs.RecordView], reported_by: str, created_at: str, resolved_by_actions: list[chitose.com.atproto.admin.defs.ActionView], reason: typing.Optional[str]=None) -> None:
+    def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoView, chitose.com.atproto.admin.defs.RepoViewNotFound, chitose.com.atproto.admin.defs.RecordView, chitose.com.atproto.admin.defs.RecordViewNotFound], reported_by: str, created_at: str, resolved_by_actions: list[chitose.com.atproto.admin.defs.ActionView], reason: typing.Optional[str]=None) -> None:
         self.id = id
         self.reason_type = reason_type
         self.subject = subject
         self.reported_by = reported_by
         self.created_at = created_at
         self.resolved_by_actions = resolved_by_actions
         self.reason = reason
 
     def to_dict(self) -> dict:
         return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActions': self.resolved_by_actions, 'reason': self.reason, '$type': 'com.atproto.admin.defs#reportViewDetail'}
 
 class RepoView(chitose.Object):
     """"""
 
-    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.Moderation, email: typing.Optional[str]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites_disabled: typing.Optional[str]=None) -> None:
+    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.Moderation, email: typing.Optional[str]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites_disabled: typing.Optional[bool]=None) -> None:
         self.did = did
         self.handle = handle
         self.related_records = related_records
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.email = email
         self.invited_by = invited_by
@@ -118,29 +118,38 @@
 
     def to_dict(self) -> dict:
         return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'invitedBy': self.invited_by, 'invitesDisabled': self.invites_disabled, '$type': 'com.atproto.admin.defs#repoView'}
 
 class RepoViewDetail(chitose.Object):
     """"""
 
-    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.ModerationDetail, email: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites: typing.Optional[list[chitose.com.atproto.server.defs.InviteCode]]=None, invites_disabled: typing.Optional[str]=None) -> None:
+    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.ModerationDetail, email: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites: typing.Optional[list[chitose.com.atproto.server.defs.InviteCode]]=None, invites_disabled: typing.Optional[bool]=None) -> None:
         self.did = did
         self.handle = handle
         self.related_records = related_records
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.email = email
         self.labels = labels
         self.invited_by = invited_by
         self.invites = invites
         self.invites_disabled = invites_disabled
 
     def to_dict(self) -> dict:
         return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'labels': self.labels, 'invitedBy': self.invited_by, 'invites': self.invites, 'invitesDisabled': self.invites_disabled, '$type': 'com.atproto.admin.defs#repoViewDetail'}
 
+class RepoViewNotFound(chitose.Object):
+    """"""
+
+    def __init__(self, did: str) -> None:
+        self.did = did
+
+    def to_dict(self) -> dict:
+        return {'did': self.did, '$type': 'com.atproto.admin.defs#repoViewNotFound'}
+
 class RepoRef(chitose.Object):
     """"""
 
     def __init__(self, did: str) -> None:
         self.did = did
 
     def to_dict(self) -> dict:
@@ -173,14 +182,23 @@
         self.moderation = moderation
         self.repo = repo
         self.labels = labels
 
     def to_dict(self) -> dict:
         return {'uri': self.uri, 'cid': self.cid, 'value': self.value, 'blobs': self.blobs, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'repo': self.repo, 'labels': self.labels, '$type': 'com.atproto.admin.defs#recordViewDetail'}
 
+class RecordViewNotFound(chitose.Object):
+    """"""
+
+    def __init__(self, uri: str) -> None:
+        self.uri = uri
+
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, '$type': 'com.atproto.admin.defs#recordViewNotFound'}
+
 class Moderation(chitose.Object):
     """"""
 
     def __init__(self, current_action: typing.Optional[chitose.com.atproto.admin.defs.ActionViewCurrent]=None) -> None:
         self.current_action = current_action
 
     def to_dict(self) -> dict:
```

### Comparing `chitose-0.0.5/chitose/com/atproto/admin/disable_invite_codes.py` & `chitose-0.0.6/chitose/com/atproto/admin/disable_invite_codes.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/admin/get_moderation_reports.py` & `chitose-0.0.6/chitose/com/atproto/admin/get_moderation_reports.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_moderation_reports(service: str, headers: dict[str, str], subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+def _get_moderation_reports(service: str, headers: dict[str, str], subject: typing.Optional[str]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """List moderation reports related to a subject."""
     return chitose.xrpc.call('com.atproto.admin.getModerationReports', [('subject', subject), ('resolved', resolved), ('actionType', action_type), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
```

### Comparing `chitose-0.0.5/chitose/com/atproto/admin/search_repos.py` & `chitose-0.0.6/chitose/com/atproto/admin/search_repos.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/admin/take_moderation_action.py` & `chitose-0.0.6/chitose/com/atproto/admin/take_moderation_action.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/identity/__init__.py` & `chitose-0.0.6/chitose/com/atproto/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/label/__init__.py` & `chitose-0.0.6/chitose/com/atproto/label/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/label/defs.py` & `chitose-0.0.6/chitose/com/atproto/label/defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     :param cts: timestamp when this label was created
 
     :param cid: optionally, CID specifying the specific version of 'uri' resource this label applies to
 
     :param neg: if true, this is a negation label, overwriting a previous label
     """
 
-    def __init__(self, src: str, uri: str, val: str, cts: str, cid: typing.Optional[str]=None, neg: typing.Optional[str]=None) -> None:
+    def __init__(self, src: str, uri: str, val: str, cts: str, cid: typing.Optional[str]=None, neg: typing.Optional[bool]=None) -> None:
         self.src = src
         self.uri = uri
         self.val = val
         self.cts = cts
         self.cid = cid
         self.neg = neg
```

### Comparing `chitose-0.0.5/chitose/com/atproto/label/query_labels.py` & `chitose-0.0.6/chitose/com/atproto/label/query_labels.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/label/subscribe_labels.py` & `chitose-0.0.6/chitose/com/atproto/label/subscribe_labels.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/moderation/__init__.py` & `chitose-0.0.6/chitose/com/atproto/moderation/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/moderation/create_report.py` & `chitose-0.0.6/chitose/com/atproto/moderation/create_report.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/moderation/defs.py` & `chitose-0.0.6/chitose/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/repo/__init__.py` & `chitose-0.0.6/chitose/com/atproto/repo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class Repo_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def create_record(self, repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+    def create_record(self, repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Create a new record.
 
 
         :param repo: The handle or DID of the repo.
 
         :param collection: The NSID of the record collection.
 
@@ -49,15 +49,15 @@
 
         :param swap_record: Compare and swap with the previous record by cid.
 
         :param swap_commit: Compare and swap with the previous commit by cid.
         """
         return _delete_record(self.service, self.headers, repo, collection, rkey, swap_record, swap_commit)
 
-    def put_record(self, repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[str]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+    def put_record(self, repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[bool]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Write a record, creating or updating it as needed.
 
 
         :param repo: The handle or DID of the repo.
 
         :param collection: The NSID of the record collection.
 
@@ -105,25 +105,25 @@
 
         :param rkey: The key of the record.
 
         :param cid: The CID of the version of the record. If not specified, then return the most recent version.
         """
         return _get_record(self.service, self.headers, repo, collection, rkey, cid)
 
-    def apply_writes(self, repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+    def apply_writes(self, repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Apply a batch transaction of creates, updates, and deletes.
 
 
         :param repo: The handle or DID of the repo.
 
         :param validate: Validate the records?
         """
         return _apply_writes(self.service, self.headers, repo, writes, validate, swap_commit)
 
-    def list_records(self, repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[str]=None) -> bytes:
+    def list_records(self, repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
         """List a range of records in a collection.
 
 
         :param repo: The handle or DID of the repo.
 
         :param collection: The NSID of the record type.
```

### Comparing `chitose-0.0.5/chitose/com/atproto/repo/apply_writes.py` & `chitose-0.0.6/chitose/com/atproto/repo/apply_writes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.repo.apply_writes
 import typing
 
-def _apply_writes(service: str, headers: dict[str, str], repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+def _apply_writes(service: str, headers: dict[str, str], repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Apply a batch transaction of creates, updates, and deletes.
 
 
     :param repo: The handle or DID of the repo.
 
     :param validate: Validate the records?
     """
```

### Comparing `chitose-0.0.5/chitose/com/atproto/repo/create_record.py` & `chitose-0.0.6/chitose/com/atproto/repo/create_record.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_record(service: str, headers: dict[str, str], repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+def _create_record(service: str, headers: dict[str, str], repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Create a new record.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
```

### Comparing `chitose-0.0.5/chitose/com/atproto/repo/delete_record.py` & `chitose-0.0.6/chitose/com/atproto/repo/delete_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/repo/get_record.py` & `chitose-0.0.6/chitose/com/atproto/repo/get_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/repo/list_records.py` & `chitose-0.0.6/chitose/com/atproto/repo/list_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _list_records(service: str, headers: dict[str, str], repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[str]=None) -> bytes:
+def _list_records(service: str, headers: dict[str, str], repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
     """List a range of records in a collection.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record type.
```

### Comparing `chitose-0.0.5/chitose/com/atproto/repo/put_record.py` & `chitose-0.0.6/chitose/com/atproto/repo/put_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _put_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[str]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+def _put_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[bool]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Write a record, creating or updating it as needed.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
```

### Comparing `chitose-0.0.5/chitose/com/atproto/repo/rebase_repo.py` & `chitose-0.0.6/chitose/com/atproto/repo/rebase_repo.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/server/__init__.py` & `chitose-0.0.6/chitose/com/atproto/server/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class Server_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def get_account_invite_codes(self, include_used: typing.Optional[str]=None, create_available: typing.Optional[str]=None) -> bytes:
+    def get_account_invite_codes(self, include_used: typing.Optional[bool]=None, create_available: typing.Optional[bool]=None) -> bytes:
         """Get all invite codes for a given account"""
         return _get_account_invite_codes(self.service, self.headers, include_used, create_available)
 
     def create_session(self, identifier: str, password: str) -> bytes:
         """Create an authentication session.
```

### Comparing `chitose-0.0.5/chitose/com/atproto/server/create_account.py` & `chitose-0.0.6/chitose/com/atproto/server/create_account.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/server/create_app_password.py` & `chitose-0.0.6/chitose/com/atproto/server/create_app_password.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/server/create_invite_codes.py` & `chitose-0.0.6/chitose/com/atproto/server/create_invite_codes.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/server/create_session.py` & `chitose-0.0.6/chitose/com/atproto/server/create_session.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/server/defs.py` & `chitose-0.0.6/chitose/com/atproto/server/defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.server.defs
 
 class InviteCode(chitose.Object):
     """"""
 
-    def __init__(self, code: str, available: int, disabled: str, for_account: str, created_by: str, created_at: str, uses: list[chitose.com.atproto.server.defs.InviteCodeUse]) -> None:
+    def __init__(self, code: str, available: int, disabled: bool, for_account: str, created_by: str, created_at: str, uses: list[chitose.com.atproto.server.defs.InviteCodeUse]) -> None:
         self.code = code
         self.available = available
         self.disabled = disabled
         self.for_account = for_account
         self.created_by = created_by
         self.created_at = created_at
         self.uses = uses
```

### Comparing `chitose-0.0.5/chitose/com/atproto/server/describe_server.py` & `chitose-0.0.6/chitose/com/atproto/server/describe_server.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/server/list_app_passwords.py` & `chitose-0.0.6/chitose/com/atproto/server/list_app_passwords.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/sync/__init__.py` & `chitose-0.0.6/chitose/com/atproto/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/sync/get_commit_path.py` & `chitose-0.0.6/chitose/com/atproto/sync/get_commit_path.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/sync/get_record.py` & `chitose-0.0.6/chitose/com/atproto/sync/get_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/sync/get_repo.py` & `chitose-0.0.6/chitose/com/atproto/sync/get_repo.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/sync/list_blobs.py` & `chitose-0.0.6/chitose/com/atproto/sync/list_blobs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/sync/list_repos.py` & `chitose-0.0.6/chitose/com/atproto/sync/list_repos.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/sync/notify_of_update.py` & `chitose-0.0.6/chitose/com/atproto/sync/notify_of_update.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/chitose/com/atproto/sync/subscribe_repos.py` & `chitose-0.0.6/chitose/com/atproto/sync/subscribe_repos.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class Commit(chitose.Object):
     """
 
 
     :param blocks: CAR file containing relevant blocks
     """
 
-    def __init__(self, seq: int, rebase: str, too_big: str, repo: str, commit: typing.Any, prev: typing.Any, blocks: typing.Any, ops: list[chitose.com.atproto.sync.subscribe_repos.RepoOp], blobs: list[typing.Any], time: str) -> None:
+    def __init__(self, seq: int, rebase: bool, too_big: bool, repo: str, commit: typing.Any, prev: typing.Any, blocks: typing.Any, ops: list[chitose.com.atproto.sync.subscribe_repos.RepoOp], blobs: list[typing.Any], time: str) -> None:
         self.seq = seq
         self.rebase = rebase
         self.too_big = too_big
         self.repo = repo
         self.commit = commit
         self.prev = prev
         self.blocks = blocks
```

### Comparing `chitose-0.0.5/LICENSE` & `chitose-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chitose-0.0.5/README.md` & `chitose-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Chitose
 
+[![Python](https://img.shields.io/pypi/pyversions/chitose.svg)](https://badge.fury.io/py/chitose)
+[![PyPI](https://badge.fury.io/py/chitose.svg)](https://badge.fury.io/py/chitose)
+[![Read the Docs](https://readthedocs.org/projects/chitose/badge/?version=latest&style=flat)](https://chitose.readthedocs.io/en/latest/)
+
 Chitose is a Python client library for the AT Protocol (Bluesky).
 
 ## Usage
 
 The API of Chitose is similar to [the ATP API](https://github.com/bluesky-social/atproto/blob/main/packages/api/README.md).
 
 For example, you can use `get_timeline()` in `BskyAgent` to get the timeline as shown below. Replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your username and your password respectively:
```

### Comparing `chitose-0.0.5/PKG-INFO` & `chitose-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: chitose
-Version: 0.0.5
+Version: 0.0.6
 Summary: A client library for the AT Protocol (Bluesky) 
-Project-URL: Homepage, https://github.com/mnogu/chitose
-Project-URL: Bug Tracker, https://github.com/mnogu/chitose/issues
-Author-email: Muneyuki Noguchi <nogu.dev@gmail.com>
-License-File: LICENSE
+Home-page: https://github.com/mnogu/chitose
+License: MIT
+Author: Muneyuki Noguchi
+Author-email: nogu.dev@gmail.com
+Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
-Requires-Python: >=3.9
+Project-URL: Documentation, https://chitose.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/mnogu/chitose
 Description-Content-Type: text/markdown
 
 # Chitose
 
+[![Python](https://img.shields.io/pypi/pyversions/chitose.svg)](https://badge.fury.io/py/chitose)
+[![PyPI](https://badge.fury.io/py/chitose.svg)](https://badge.fury.io/py/chitose)
+[![Read the Docs](https://readthedocs.org/projects/chitose/badge/?version=latest&style=flat)](https://chitose.readthedocs.io/en/latest/)
+
 Chitose is a Python client library for the AT Protocol (Bluesky).
 
 ## Usage
 
 The API of Chitose is similar to [the ATP API](https://github.com/bluesky-social/atproto/blob/main/packages/api/README.md).
 
 For example, you can use `get_timeline()` in `BskyAgent` to get the timeline as shown below. Replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your username and your password respectively:
@@ -105,8 +114,8 @@
 $ git add chitose
 $ git commit
 ```
 ```
 $ python3 -m pip install sphinx
 $ cd docs
 $ sphinx-apidoc -o ./source ../chitose -f
-```
+```
```

