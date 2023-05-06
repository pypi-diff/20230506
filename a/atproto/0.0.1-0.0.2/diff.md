# Comparing `tmp/atproto-0.0.1.tar.gz` & `tmp/atproto-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atproto-0.0.1.tar", max compression
+gzip compressed data, was "atproto-0.0.2.tar", max compression
```

## Comparing `atproto-0.0.1.tar` & `atproto-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,151 @@
--rw-r--r--   0        0        0     1061 2022-11-22 23:49:44.257038 atproto-0.0.1/LICENSE
--rw-r--r--   0        0        0       20 2022-11-22 23:51:05.034490 atproto-0.0.1/README.md
--rw-r--r--   0        0        0        0 2022-11-23 00:05:34.822632 atproto-0.0.1/atproto/__init__.py
--rw-r--r--   0        0        0     1320 2022-11-22 23:54:22.469951 atproto-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 atproto-0.0.1/setup.py
--rw-r--r--   0        0        0     1283 1970-01-01 00:00:00.000000 atproto-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-06 18:19:17.839834 atproto-0.0.2/LICENSE
+-rw-r--r--   0        0        0     9736 2023-05-06 18:19:17.839834 atproto-0.0.2/README.md
+-rw-r--r--   0        0        0      300 2023-05-06 18:19:17.839834 atproto-0.0.2/atproto/__init__.py
+-rw-r--r--   0        0        0      619 2023-05-06 18:19:17.839834 atproto-0.0.2/atproto/cid/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-06 18:19:17.839834 atproto-0.0.2/atproto/cli/__init__.py
+-rw-r--r--   0        0        0     2767 2023-05-06 18:19:17.839834 atproto-0.0.2/atproto/codegen/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/clients/__init__.py
+-rw-r--r--   0        0        0     1156 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/clients/generate_async_client.py
+-rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/models/__init__.py
+-rw-r--r--   0        0        0     2317 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/models/builder.py
+-rw-r--r--   0        0        0    17423 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/models/generator.py
+-rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/namespaces/__init__.py
+-rw-r--r--   0        0        0     2562 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/namespaces/builder.py
+-rw-r--r--   0        0        0    11855 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/namespaces/generator.py
+-rw-r--r--   0        0        0      891 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/lexicon/__init__.py
+-rw-r--r--   0        0        0     4658 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/lexicon/models.py
+-rw-r--r--   0        0        0     3871 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/lexicon/parser.py
+-rw-r--r--   0        0        0     5298 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/nsid/__init__.py
+-rw-r--r--   0        0        0     3075 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/uri/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/__init__.py
+-rw-r--r--   0        0        0     5994 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/async_client.py
+-rw-r--r--   0        0        0      489 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/async_raw.py
+-rw-r--r--   0        0        0     3719 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/base.py
+-rw-r--r--   0        0        0     5555 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/client.py
+-rw-r--r--   0        0        0      469 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/raw.py
+-rw-r--r--   0        0        0    10098 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     3057 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      836 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      890 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0     1014 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      927 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0     1061 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      970 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1619 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1417 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2163 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1145 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     3776 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0     1041 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0     1449 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0     1039 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      855 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0     1181 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0     1066 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      734 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2257 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      738 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      665 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/block.py
+-rw-r--r--   0        0        0      667 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0     1004 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0     1133 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0     1123 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      999 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0      574 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      576 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      830 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1845 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      586 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1551 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0     1082 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      297 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/base.py
+-rw-r--r--   0        0        0      713 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/blob_ref.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0     8856 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      712 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0     1071 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      839 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0     1097 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      839 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0     1161 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      890 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      824 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      953 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      911 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0     1129 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1341 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      651 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      621 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      887 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      586 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1191 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/defs.py
+-rw-r--r--   0        0        0     1323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0      957 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0     1452 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      825 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     1898 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0     1222 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      969 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0     1024 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0     1157 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1747 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1305 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      644 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      742 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      983 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      880 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0     1282 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0     1117 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1183 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      659 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0     1211 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0     1028 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      704 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      956 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      729 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      589 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      628 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      583 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      752 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      744 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      822 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      986 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      764 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      872 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      916 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      969 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0     1201 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      637 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      640 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2426 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0     2810 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/utils.py
+-rw-r--r--   0        0        0        0 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/namespaces/__init__.py
+-rw-r--r--   0        0        0    65433 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/namespaces/async_ns.py
+-rw-r--r--   0        0        0      361 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/namespaces/base.py
+-rw-r--r--   0        0        0    64495 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/namespaces/sync_ns.py
+-rw-r--r--   0        0        0     4353 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/request.py
+-rw-r--r--   0        0        0       43 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_server/__init__.py
+-rw-r--r--   0        0        0     2083 2023-05-06 18:19:17.859834 atproto-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11556 1970-01-01 00:00:00.000000 atproto-0.0.2/PKG-INFO
```

### Comparing `atproto-0.0.1/LICENSE` & `atproto-0.0.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Ilya
+Copyright (c) 2023 Ilya
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

