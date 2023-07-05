# Comparing `tmp/swibots-1.3.0.tar.gz` & `tmp/swibots-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swibots-1.3.0.tar", last modified: Tue Jul  4 10:10:22 2023, max compression
+gzip compressed data, was "swibots-1.3.1.tar", last modified: Wed Jul  5 10:07:31 2023, max compression
```

## Comparing `swibots-1.3.0.tar` & `swibots-1.3.1.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.672151 swibots-1.3.0/
--rw-rw-rw-   0        0        0     1892 2023-07-04 10:10:22.670155 swibots-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1601 2023-06-26 07:52:28.000000 swibots-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 10:10:22.672151 swibots-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-07-04 08:17:17.000000 swibots-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.096545 swibots-1.3.0/swibots/
--rw-rw-rw-   0        0        0      247 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.118543 swibots-1.3.0/swibots/api/
--rw-rw-rw-   0        0        0      146 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/__init__.py
--rw-rw-rw-   0        0        0     2317 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/api_client.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.123543 swibots-1.3.0/swibots/api/auth/
--rw-rw-rw-   0        0        0       88 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/auth/__init__.py
--rw-rw-rw-   0        0        0     1258 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/auth/auth_client.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.129553 swibots-1.3.0/swibots/api/auth/controllers/
--rw-rw-rw-   0        0        0       75 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/auth/controllers/__init__.py
--rw-rw-rw-   0        0        0     1565 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/auth/controllers/user_controller.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.137546 swibots-1.3.0/swibots/api/auth/methods/
--rw-rw-rw-   0        0        0       99 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/auth/methods/__init__.py
--rw-rw-rw-   0        0        0      671 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/auth/methods/get_me.py
--rw-rw-rw-   0        0        0      861 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/auth/methods/login.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.143566 swibots-1.3.0/swibots/api/auth/models/
--rw-rw-rw-   0        0        0       59 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/auth/models/__init__.py
--rw-rw-rw-   0        0        0     4765 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/auth/models/auth_user.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.149545 swibots-1.3.0/swibots/api/bot/
--rw-rw-rw-   0        0        0       86 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/__init__.py
--rw-rw-rw-   0        0        0     1177 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/bot_client.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.155544 swibots-1.3.0/swibots/api/bot/controllers/
--rw-rw-rw-   0        0        0       74 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/controllers/__init__.py
--rw-rw-rw-   0        0        0     1852 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/controllers/bot_controller.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.167544 swibots-1.3.0/swibots/api/bot/methods/
--rw-rw-rw-   0        0        0      220 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/methods/__init__.py
--rw-rw-rw-   0        0        0      557 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/methods/delete_bot_info.py
--rw-rw-rw-   0        0        0      600 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/methods/get_bot_info.py
--rw-rw-rw-   0        0        0      633 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/methods/update_bot_info.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.176547 swibots-1.3.0/swibots/api/bot/models/
--rw-rw-rw-   0        0        0      120 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/models/__init__.py
--rw-rw-rw-   0        0        0      987 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/models/bot_command_info.py
--rw-rw-rw-   0        0        0     1633 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/bot/models/bot_info.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.181552 swibots-1.3.0/swibots/api/chat/
--rw-rw-rw-   0        0        0      111 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/__init__.py
--rw-rw-rw-   0        0        0     5512 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/chat_client.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.188546 swibots-1.3.0/swibots/api/chat/controllers/
--rw-rw-rw-   0        0        0       86 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/controllers/__init__.py
--rw-rw-rw-   0        0        0    22044 2023-06-26 12:37:56.000000 swibots-1.3.0/swibots/api/chat/controllers/message_controller.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.207546 swibots-1.3.0/swibots/api/chat/events/
--rw-rw-rw-   0        0        0      334 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/events/__init__.py
--rw-rw-rw-   0        0        0     2134 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/events/callback_query_event.py
--rw-rw-rw-   0        0        0     2809 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/events/chat_event.py
--rw-rw-rw-   0        0        0     2157 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/events/command_event.py
--rw-rw-rw-   0        0        0     2166 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/events/inline_query_event.py
--rw-rw-rw-   0        0        0     2503 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/events/message_event.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.291626 swibots-1.3.0/swibots/api/chat/methods/
--rw-rw-rw-   0        0        0     1761 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/__init__.py
--rw-rw-rw-   0        0        0      668 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/answer_inline_query.py
--rw-rw-rw-   0        0        0      714 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/clear_conversation.py
--rw-rw-rw-   0        0        0      726 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/delete_message.py
--rw-rw-rw-   0        0        0      728 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/delete_messages_from_user.py
--rw-rw-rw-   0        0        0     1392 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/download_media.py
--rw-rw-rw-   0        0        0      774 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/edit_message.py
--rw-rw-rw-   0        0        0      877 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/edit_message_text.py
--rw-rw-rw-   0        0        0      714 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/flag_message.py
--rw-rw-rw-   0        0        0     1223 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/forward_message.py
--rw-rw-rw-   0        0        0     1172 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/get_channel_chat_history.py
--rw-rw-rw-   0        0        0      748 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/get_community_media_files.py
--rw-rw-rw-   0        0        0      909 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/get_community_media_files_by_status.py
--rw-rw-rw-   0        0        0      655 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/get_flag_messages.py
--rw-rw-rw-   0        0        0     1122 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/get_group_chat_history.py
--rw-rw-rw-   0        0        0      670 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/get_message.py
--rw-rw-rw-   0        0        0      728 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/get_messages.py
--rw-rw-rw-   0        0        0     1134 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/get_messages_between_users.py
--rw-rw-rw-   0        0        0      576 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/get_unread_messages_count.py
--rw-rw-rw-   0        0        0      810 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/get_user_media_files.py
--rw-rw-rw-   0        0        0      906 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/reply_message.py
--rw-rw-rw-   0        0        0     1058 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/reply_message_text.py
--rw-rw-rw-   0        0        0      874 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/send_message.py
--rw-rw-rw-   0        0        0     1163 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/methods/send_text.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.318627 swibots-1.3.0/swibots/api/chat/models/
--rw-rw-rw-   0        0        0      312 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/__init__.py
--rw-rw-rw-   0        0        0      951 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/group_chat_history.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.361627 swibots-1.3.0/swibots/api/chat/models/inline/
--rw-rw-rw-   0        0        0      575 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/__init__.py
--rw-rw-rw-   0        0        0     1410 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/base_typed_inline_query_result.py
--rw-rw-rw-   0        0        0     2605 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/inline_query.py
--rw-rw-rw-   0        0        0     1931 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/inline_query_answer.py
--rw-rw-rw-   0        0        0     1021 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/inline_query_result.py
--rw-rw-rw-   0        0        0     1190 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/inline_query_result_article.py
--rw-rw-rw-   0        0        0     1308 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/inline_query_result_document.py
--rw-rw-rw-   0        0        0     1664 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/inline_query_result_photo.py
--rw-rw-rw-   0        0        0     1807 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/inline_query_result_video.py
--rw-rw-rw-   0        0        0      603 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/input_message_content.py
--rw-rw-rw-   0        0        0      211 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline/types.py
--rw-rw-rw-   0        0        0      919 2023-07-04 08:08:33.000000 swibots-1.3.0/swibots/api/chat/models/inline_keyboard_button.py
--rw-rw-rw-   0        0        0      180 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline_keyboard_color.py
--rw-rw-rw-   0        0        0      154 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/chat/models/inline_keyboard_size.py
--rw-rw-rw-   0        0        0     3007 2023-07-04 08:43:22.000000 swibots-1.3.0/swibots/api/chat/models/inline_markup.py
--rw-rw-rw-   0        0        0    12553 2023-07-04 10:01:19.000000 swibots-1.3.0/swibots/api/chat/models/message.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.364623 swibots-1.3.0/swibots/api/common/
--rw-rw-rw-   0        0        0       46 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.370627 swibots-1.3.0/swibots/api/common/events/
--rw-rw-rw-   0        0        0       49 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/common/events/__init__.py
--rw-rw-rw-   0        0        0     2859 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/common/events/event.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.382620 swibots-1.3.0/swibots/api/common/models/
--rw-rw-rw-   0        0        0      104 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/common/models/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/common/models/media.py
--rw-rw-rw-   0        0        0     1624 2023-06-26 12:38:24.000000 swibots-1.3.0/swibots/api/common/models/media_upload_request.py
--rw-rw-rw-   0        0        0     1759 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/common/models/user.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.387620 swibots-1.3.0/swibots/api/community/
--rw-rw-rw-   0        0        0       93 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/__init__.py
--rw-rw-rw-   0        0        0     5180 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/community_client.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.399620 swibots-1.3.0/swibots/api/community/controllers/
--rw-rw-rw-   0        0        0      105 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/controllers/__init__.py
--rw-rw-rw-   0        0        0      618 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/controllers/channel_controller.py
--rw-rw-rw-   0        0        0      636 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/controllers/community_controller.py
--rw-rw-rw-   0        0        0      596 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/controllers/group_controller.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.445618 swibots-1.3.0/swibots/api/community/events/
--rw-rw-rw-   0        0        0      577 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/channel_created_event.py
--rw-rw-rw-   0        0        0     1428 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/channel_deleted_event.py
--rw-rw-rw-   0        0        0     1428 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/channel_updated_event.py
--rw-rw-rw-   0        0        0     2373 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/community_event.py
--rw-rw-rw-   0        0        0     1424 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/community_updated_event.py
--rw-rw-rw-   0        0        0     1422 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/group_created_event.py
--rw-rw-rw-   0        0        0     1422 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/group_deleted_event.py
--rw-rw-rw-   0        0        0     1422 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/group_updated_event.py
--rw-rw-rw-   0        0        0     1421 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/member_joined_event.py
--rw-rw-rw-   0        0        0     1418 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/member_left_event.py
--rw-rw-rw-   0        0        0     1414 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/events/user_banned_event.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.462161 swibots-1.3.0/swibots/api/community/methods/
--rw-rw-rw-   0        0        0      205 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/methods/__init__.py
--rw-rw-rw-   0        0        0      664 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/methods/get_channel.py
--rw-rw-rw-   0        0        0      689 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/methods/get_community.py
--rw-rw-rw-   0        0        0      640 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/methods/get_group.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.474159 swibots-1.3.0/swibots/api/community/models/
--rw-rw-rw-   0        0        0      137 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/models/__init__.py
--rw-rw-rw-   0        0        0     2814 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/models/channel.py
--rw-rw-rw-   0        0        0     3033 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/models/community.py
--rw-rw-rw-   0        0        0     2792 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/api/community/models/group.py
--rw-rw-rw-   0        0        0     9630 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/app.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.501156 swibots-1.3.0/swibots/base/
--rw-rw-rw-   0        0        0      268 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/base/__init__.py
--rw-rw-rw-   0        0        0       71 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/base/rest_controller.py
--rw-rw-rw-   0        0        0      386 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/base/rest_request.py
--rw-rw-rw-   0        0        0      669 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/base/rest_response.py
--rw-rw-rw-   0        0        0     4380 2023-06-26 11:37:39.000000 swibots-1.3.0/swibots/base/switch_client.py
--rw-rw-rw-   0        0        0     1221 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/base/switch_object.py
--rw-rw-rw-   0        0        0      563 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/base/switch_ws_async_client.py
--rw-rw-rw-   0        0        0     4734 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bot_app.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.519152 swibots-1.3.0/swibots/bots/
--rw-rw-rw-   0        0        0      208 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/__init__.py
--rw-rw-rw-   0        0        0     4782 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/bot.py
--rw-rw-rw-   0        0        0     1690 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/bot_context.py
--rw-rw-rw-   0        0        0      111 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.568150 swibots-1.3.0/swibots/bots/decorators/
--rw-rw-rw-   0        0        0     1034 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/__init__.py
--rw-rw-rw-   0        0        0      558 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_callback_query.py
--rw-rw-rw-   0        0        0      526 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_channel_created.py
--rw-rw-rw-   0        0        0      562 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_channel_deleted.py
--rw-rw-rw-   0        0        0      559 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_channel_updated.py
--rw-rw-rw-   0        0        0      593 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_command.py
--rw-rw-rw-   0        0        0      562 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_community_updated.py
--rw-rw-rw-   0        0        0      554 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_group_created.py
--rw-rw-rw-   0        0        0      554 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_group_deleted.py
--rw-rw-rw-   0        0        0      552 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_group_updated.py
--rw-rw-rw-   0        0        0      554 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_inline_query.py
--rw-rw-rw-   0        0        0      552 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_member_joined.py
--rw-rw-rw-   0        0        0      547 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_member_left.py
--rw-rw-rw-   0        0        0      519 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_message.py
--rw-rw-rw-   0        0        0      561 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_unknown_command.py
--rw-rw-rw-   0        0        0      525 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/decorators/on_user_banned.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.574147 swibots-1.3.0/swibots/bots/filters/
--rw-rw-rw-   0        0        0       23 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/filters/__init__.py
--rw-rw-rw-   0        0        0     8057 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/filters/filter.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.633366 swibots-1.3.0/swibots/bots/handlers/
--rw-rw-rw-   0        0        0     1337 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/__init__.py
--rw-rw-rw-   0        0        0     1087 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/base_handler.py
--rw-rw-rw-   0        0        0     1016 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/callback_query_handler.py
--rw-rw-rw-   0        0        0      704 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/channel_created_handler.py
--rw-rw-rw-   0        0        0      711 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/channel_deleted_handler.py
--rw-rw-rw-   0        0        0      758 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/channel_updated_handler.py
--rw-rw-rw-   0        0        0     1557 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/command_handler.py
--rw-rw-rw-   0        0        0      709 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/community_updated_handler.py
--rw-rw-rw-   0        0        0     1365 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/event_handler.py
--rw-rw-rw-   0        0        0      703 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/group_created_handler.py
--rw-rw-rw-   0        0        0      800 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/group_deleted_handler.py
--rw-rw-rw-   0        0        0      800 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/group_updated_handler.py
--rw-rw-rw-   0        0        0      896 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/inline_query_handler.py
--rw-rw-rw-   0        0        0      702 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/member_joined_handler.py
--rw-rw-rw-   0        0        0      697 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/member_left_handler.py
--rw-rw-rw-   0        0        0      991 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/message_handler.py
--rw-rw-rw-   0        0        0      914 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/unknown_command_handler.py
--rw-rw-rw-   0        0        0      693 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/handlers/user_banned_handler.py
--rw-rw-rw-   0        0        0      298 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/bots/register_command.py
--rw-rw-rw-   0        0        0     1664 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/config.py
--rw-rw-rw-   0        0        0     1387 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/error.py
--rw-rw-rw-   0        0        0      878 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/types.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.641155 swibots-1.3.0/swibots/utils/
--rw-rw-rw-   0        0        0       78 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/utils/__init__.py
--rw-rw-rw-   0        0        0     6030 2023-06-26 11:43:01.000000 swibots-1.3.0/swibots/utils/rest_client.py
--rw-rw-rw-   0        0        0     2558 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.645152 swibots-1.3.0/swibots/utils/ws/
--rw-rw-rw-   0        0        0       50 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/utils/ws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.656153 swibots-1.3.0/swibots/utils/ws/asyncstomp/
--rw-rw-rw-   0        0        0      154 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/utils/ws/asyncstomp/__init__.py
--rw-rw-rw-   0        0        0    10071 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/utils/ws/asyncstomp/async_ws_client.py
--rw-rw-rw-   0        0        0     1010 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/utils/ws/asyncstomp/async_ws_subscription.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.666158 swibots-1.3.0/swibots/utils/ws/common/
--rw-rw-rw-   0        0        0      104 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/utils/ws/common/__init__.py
--rw-rw-rw-   0        0        0     1716 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/utils/ws/common/ws_frame.py
--rw-rw-rw-   0        0        0      441 2023-06-26 07:52:28.000000 swibots-1.3.0/swibots/utils/ws/common/ws_message.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:10:22.112551 swibots-1.3.0/swibots.egg-info/
--rw-rw-rw-   0        0        0     1892 2023-07-04 10:10:21.000000 swibots-1.3.0/swibots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7283 2023-07-04 10:10:21.000000 swibots-1.3.0/swibots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 10:10:21.000000 swibots-1.3.0/swibots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-04 10:10:21.000000 swibots-1.3.0/swibots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 10:10:21.000000 swibots-1.3.0/swibots.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.677254 swibots-1.3.1/
+-rw-rw-rw-   0        0        0     1892 2023-07-05 10:07:31.675256 swibots-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1601 2023-06-26 07:52:28.000000 swibots-1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 10:07:31.677254 swibots-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-07-05 09:48:27.000000 swibots-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.227015 swibots-1.3.1/swibots/
+-rw-rw-rw-   0        0        0      247 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.244014 swibots-1.3.1/swibots/api/
+-rw-rw-rw-   0        0        0      146 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/__init__.py
+-rw-rw-rw-   0        0        0     2317 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/api_client.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.247014 swibots-1.3.1/swibots/api/auth/
+-rw-rw-rw-   0        0        0       88 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/auth/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/auth/auth_client.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.252013 swibots-1.3.1/swibots/api/auth/controllers/
+-rw-rw-rw-   0        0        0       75 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/auth/controllers/__init__.py
+-rw-rw-rw-   0        0        0     1569 2023-07-04 10:27:05.000000 swibots-1.3.1/swibots/api/auth/controllers/user_controller.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.260015 swibots-1.3.1/swibots/api/auth/methods/
+-rw-rw-rw-   0        0        0       99 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/auth/methods/__init__.py
+-rw-rw-rw-   0        0        0      671 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/auth/methods/get_me.py
+-rw-rw-rw-   0        0        0      861 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/auth/methods/login.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.264014 swibots-1.3.1/swibots/api/auth/models/
+-rw-rw-rw-   0        0        0       59 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/auth/models/__init__.py
+-rw-rw-rw-   0        0        0     4765 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/auth/models/auth_user.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.268014 swibots-1.3.1/swibots/api/bot/
+-rw-rw-rw-   0        0        0       86 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/__init__.py
+-rw-rw-rw-   0        0        0     1177 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/bot_client.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.273018 swibots-1.3.1/swibots/api/bot/controllers/
+-rw-rw-rw-   0        0        0       74 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/controllers/__init__.py
+-rw-rw-rw-   0        0        0     1852 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/controllers/bot_controller.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.283016 swibots-1.3.1/swibots/api/bot/methods/
+-rw-rw-rw-   0        0        0      220 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/methods/__init__.py
+-rw-rw-rw-   0        0        0      557 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/methods/delete_bot_info.py
+-rw-rw-rw-   0        0        0      600 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/methods/get_bot_info.py
+-rw-rw-rw-   0        0        0      633 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/methods/update_bot_info.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.298017 swibots-1.3.1/swibots/api/bot/models/
+-rw-rw-rw-   0        0        0      120 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/models/__init__.py
+-rw-rw-rw-   0        0        0      987 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/models/bot_command_info.py
+-rw-rw-rw-   0        0        0     1633 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/bot/models/bot_info.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.328016 swibots-1.3.1/swibots/api/chat/
+-rw-rw-rw-   0        0        0      111 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/__init__.py
+-rw-rw-rw-   0        0        0     5512 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/chat_client.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.340019 swibots-1.3.1/swibots/api/chat/controllers/
+-rw-rw-rw-   0        0        0       86 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/controllers/__init__.py
+-rw-rw-rw-   0        0        0    22044 2023-06-26 12:37:56.000000 swibots-1.3.1/swibots/api/chat/controllers/message_controller.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.365019 swibots-1.3.1/swibots/api/chat/events/
+-rw-rw-rw-   0        0        0      334 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/events/__init__.py
+-rw-rw-rw-   0        0        0     2134 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/events/callback_query_event.py
+-rw-rw-rw-   0        0        0     2809 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/events/chat_event.py
+-rw-rw-rw-   0        0        0     2157 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/events/command_event.py
+-rw-rw-rw-   0        0        0     2166 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/events/inline_query_event.py
+-rw-rw-rw-   0        0        0     2503 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/events/message_event.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.423015 swibots-1.3.1/swibots/api/chat/methods/
+-rw-rw-rw-   0        0        0     1761 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/answer_inline_query.py
+-rw-rw-rw-   0        0        0      714 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/clear_conversation.py
+-rw-rw-rw-   0        0        0      726 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/delete_message.py
+-rw-rw-rw-   0        0        0      728 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/delete_messages_from_user.py
+-rw-rw-rw-   0        0        0     1392 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/download_media.py
+-rw-rw-rw-   0        0        0      774 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/edit_message.py
+-rw-rw-rw-   0        0        0      877 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/edit_message_text.py
+-rw-rw-rw-   0        0        0      714 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/flag_message.py
+-rw-rw-rw-   0        0        0     1223 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/forward_message.py
+-rw-rw-rw-   0        0        0     1172 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/get_channel_chat_history.py
+-rw-rw-rw-   0        0        0      748 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/get_community_media_files.py
+-rw-rw-rw-   0        0        0      909 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/get_community_media_files_by_status.py
+-rw-rw-rw-   0        0        0      655 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/get_flag_messages.py
+-rw-rw-rw-   0        0        0     1122 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/get_group_chat_history.py
+-rw-rw-rw-   0        0        0      670 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/get_message.py
+-rw-rw-rw-   0        0        0      728 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/get_messages.py
+-rw-rw-rw-   0        0        0     1134 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/get_messages_between_users.py
+-rw-rw-rw-   0        0        0      576 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/get_unread_messages_count.py
+-rw-rw-rw-   0        0        0      810 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/get_user_media_files.py
+-rw-rw-rw-   0        0        0      906 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/reply_message.py
+-rw-rw-rw-   0        0        0     1058 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/reply_message_text.py
+-rw-rw-rw-   0        0        0      874 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/send_message.py
+-rw-rw-rw-   0        0        0     1163 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/methods/send_text.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.440014 swibots-1.3.1/swibots/api/chat/models/
+-rw-rw-rw-   0        0        0      312 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/__init__.py
+-rw-rw-rw-   0        0        0      951 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/group_chat_history.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.466013 swibots-1.3.1/swibots/api/chat/models/inline/
+-rw-rw-rw-   0        0        0      575 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/__init__.py
+-rw-rw-rw-   0        0        0     1410 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/base_typed_inline_query_result.py
+-rw-rw-rw-   0        0        0     2605 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/inline_query.py
+-rw-rw-rw-   0        0        0     1931 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/inline_query_answer.py
+-rw-rw-rw-   0        0        0     1021 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/inline_query_result.py
+-rw-rw-rw-   0        0        0     1190 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/inline_query_result_article.py
+-rw-rw-rw-   0        0        0     1308 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/inline_query_result_document.py
+-rw-rw-rw-   0        0        0     1664 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/inline_query_result_photo.py
+-rw-rw-rw-   0        0        0     1807 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/inline_query_result_video.py
+-rw-rw-rw-   0        0        0      603 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/input_message_content.py
+-rw-rw-rw-   0        0        0      211 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline/types.py
+-rw-rw-rw-   0        0        0      884 2023-07-05 10:00:20.000000 swibots-1.3.1/swibots/api/chat/models/inline_keyboard_button.py
+-rw-rw-rw-   0        0        0      180 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline_keyboard_color.py
+-rw-rw-rw-   0        0        0      154 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/chat/models/inline_keyboard_size.py
+-rw-rw-rw-   0        0        0     2934 2023-07-05 10:03:12.000000 swibots-1.3.1/swibots/api/chat/models/inline_markup.py
+-rw-rw-rw-   0        0        0    12553 2023-07-04 10:01:19.000000 swibots-1.3.1/swibots/api/chat/models/message.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.468012 swibots-1.3.1/swibots/api/common/
+-rw-rw-rw-   0        0        0       46 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.472014 swibots-1.3.1/swibots/api/common/events/
+-rw-rw-rw-   0        0        0       49 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/common/events/__init__.py
+-rw-rw-rw-   0        0        0     2859 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/common/events/event.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.481015 swibots-1.3.1/swibots/api/common/models/
+-rw-rw-rw-   0        0        0      104 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/common/models/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/common/models/media.py
+-rw-rw-rw-   0        0        0     1624 2023-06-26 12:38:24.000000 swibots-1.3.1/swibots/api/common/models/media_upload_request.py
+-rw-rw-rw-   0        0        0     1759 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/common/models/user.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.485015 swibots-1.3.1/swibots/api/community/
+-rw-rw-rw-   0        0        0       93 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/__init__.py
+-rw-rw-rw-   0        0        0     5180 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/community_client.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.495014 swibots-1.3.1/swibots/api/community/controllers/
+-rw-rw-rw-   0        0        0      105 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/controllers/__init__.py
+-rw-rw-rw-   0        0        0      618 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/controllers/channel_controller.py
+-rw-rw-rw-   0        0        0      636 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/controllers/community_controller.py
+-rw-rw-rw-   0        0        0      596 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/controllers/group_controller.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.521014 swibots-1.3.1/swibots/api/community/events/
+-rw-rw-rw-   0        0        0      577 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/channel_created_event.py
+-rw-rw-rw-   0        0        0     1428 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/channel_deleted_event.py
+-rw-rw-rw-   0        0        0     1428 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/channel_updated_event.py
+-rw-rw-rw-   0        0        0     2373 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/community_event.py
+-rw-rw-rw-   0        0        0     1424 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/community_updated_event.py
+-rw-rw-rw-   0        0        0     1422 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/group_created_event.py
+-rw-rw-rw-   0        0        0     1422 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/group_deleted_event.py
+-rw-rw-rw-   0        0        0     1422 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/group_updated_event.py
+-rw-rw-rw-   0        0        0     1421 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/member_joined_event.py
+-rw-rw-rw-   0        0        0     1418 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/member_left_event.py
+-rw-rw-rw-   0        0        0     1414 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/events/user_banned_event.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.531015 swibots-1.3.1/swibots/api/community/methods/
+-rw-rw-rw-   0        0        0      205 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/methods/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/methods/get_channel.py
+-rw-rw-rw-   0        0        0      689 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/methods/get_community.py
+-rw-rw-rw-   0        0        0      640 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/methods/get_group.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.540014 swibots-1.3.1/swibots/api/community/models/
+-rw-rw-rw-   0        0        0      137 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/models/__init__.py
+-rw-rw-rw-   0        0        0     2814 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/models/channel.py
+-rw-rw-rw-   0        0        0     3033 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/models/community.py
+-rw-rw-rw-   0        0        0     2792 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/api/community/models/group.py
+-rw-rw-rw-   0        0        0     9630 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/app.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.555243 swibots-1.3.1/swibots/base/
+-rw-rw-rw-   0        0        0      268 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/base/__init__.py
+-rw-rw-rw-   0        0        0       71 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/base/rest_controller.py
+-rw-rw-rw-   0        0        0      386 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/base/rest_request.py
+-rw-rw-rw-   0        0        0      669 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/base/rest_response.py
+-rw-rw-rw-   0        0        0     4380 2023-06-26 11:37:39.000000 swibots-1.3.1/swibots/base/switch_client.py
+-rw-rw-rw-   0        0        0     1221 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/base/switch_object.py
+-rw-rw-rw-   0        0        0      563 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/base/switch_ws_async_client.py
+-rw-rw-rw-   0        0        0     4734 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bot_app.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.566255 swibots-1.3.1/swibots/bots/
+-rw-rw-rw-   0        0        0      208 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/__init__.py
+-rw-rw-rw-   0        0        0     4782 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/bot.py
+-rw-rw-rw-   0        0        0     1690 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/bot_context.py
+-rw-rw-rw-   0        0        0      111 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.603254 swibots-1.3.1/swibots/bots/decorators/
+-rw-rw-rw-   0        0        0     1034 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_callback_query.py
+-rw-rw-rw-   0        0        0      526 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_channel_created.py
+-rw-rw-rw-   0        0        0      562 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_channel_deleted.py
+-rw-rw-rw-   0        0        0      559 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_channel_updated.py
+-rw-rw-rw-   0        0        0      593 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_command.py
+-rw-rw-rw-   0        0        0      562 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_community_updated.py
+-rw-rw-rw-   0        0        0      554 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_group_created.py
+-rw-rw-rw-   0        0        0      554 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_group_deleted.py
+-rw-rw-rw-   0        0        0      552 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_group_updated.py
+-rw-rw-rw-   0        0        0      554 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_inline_query.py
+-rw-rw-rw-   0        0        0      552 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_member_joined.py
+-rw-rw-rw-   0        0        0      547 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_member_left.py
+-rw-rw-rw-   0        0        0      519 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_message.py
+-rw-rw-rw-   0        0        0      561 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_unknown_command.py
+-rw-rw-rw-   0        0        0      525 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/decorators/on_user_banned.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.607255 swibots-1.3.1/swibots/bots/filters/
+-rw-rw-rw-   0        0        0       23 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/filters/__init__.py
+-rw-rw-rw-   0        0        0     8057 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/filters/filter.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.650257 swibots-1.3.1/swibots/bots/handlers/
+-rw-rw-rw-   0        0        0     1337 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1087 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/base_handler.py
+-rw-rw-rw-   0        0        0     1016 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/callback_query_handler.py
+-rw-rw-rw-   0        0        0      704 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/channel_created_handler.py
+-rw-rw-rw-   0        0        0      711 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/channel_deleted_handler.py
+-rw-rw-rw-   0        0        0      758 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/channel_updated_handler.py
+-rw-rw-rw-   0        0        0     1557 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/command_handler.py
+-rw-rw-rw-   0        0        0      709 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/community_updated_handler.py
+-rw-rw-rw-   0        0        0     1365 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/event_handler.py
+-rw-rw-rw-   0        0        0      703 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/group_created_handler.py
+-rw-rw-rw-   0        0        0      800 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/group_deleted_handler.py
+-rw-rw-rw-   0        0        0      800 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/group_updated_handler.py
+-rw-rw-rw-   0        0        0      896 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/inline_query_handler.py
+-rw-rw-rw-   0        0        0      702 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/member_joined_handler.py
+-rw-rw-rw-   0        0        0      697 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/member_left_handler.py
+-rw-rw-rw-   0        0        0      991 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/message_handler.py
+-rw-rw-rw-   0        0        0      914 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/unknown_command_handler.py
+-rw-rw-rw-   0        0        0      693 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/handlers/user_banned_handler.py
+-rw-rw-rw-   0        0        0      298 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/bots/register_command.py
+-rw-rw-rw-   0        0        0     1686 2023-07-04 10:34:26.000000 swibots-1.3.1/swibots/config.py
+-rw-rw-rw-   0        0        0     1387 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/error.py
+-rw-rw-rw-   0        0        0      878 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/types.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.656256 swibots-1.3.1/swibots/utils/
+-rw-rw-rw-   0        0        0       78 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/utils/__init__.py
+-rw-rw-rw-   0        0        0     6030 2023-06-26 11:43:01.000000 swibots-1.3.1/swibots/utils/rest_client.py
+-rw-rw-rw-   0        0        0     2558 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.659256 swibots-1.3.1/swibots/utils/ws/
+-rw-rw-rw-   0        0        0       50 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/utils/ws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.665252 swibots-1.3.1/swibots/utils/ws/asyncstomp/
+-rw-rw-rw-   0        0        0      154 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/utils/ws/asyncstomp/__init__.py
+-rw-rw-rw-   0        0        0    10071 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/utils/ws/asyncstomp/async_ws_client.py
+-rw-rw-rw-   0        0        0     1010 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/utils/ws/asyncstomp/async_ws_subscription.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.673254 swibots-1.3.1/swibots/utils/ws/common/
+-rw-rw-rw-   0        0        0      104 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/utils/ws/common/__init__.py
+-rw-rw-rw-   0        0        0     1716 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/utils/ws/common/ws_frame.py
+-rw-rw-rw-   0        0        0      441 2023-06-26 07:52:28.000000 swibots-1.3.1/swibots/utils/ws/common/ws_message.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:31.238017 swibots-1.3.1/swibots.egg-info/
+-rw-rw-rw-   0        0        0     1892 2023-07-05 10:07:30.000000 swibots-1.3.1/swibots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7283 2023-07-05 10:07:31.000000 swibots-1.3.1/swibots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 10:07:30.000000 swibots-1.3.1/swibots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-05 10:07:30.000000 swibots-1.3.1/swibots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-05 10:07:30.000000 swibots-1.3.1/swibots.egg-info/top_level.txt
```

### Comparing `swibots-1.3.0/PKG-INFO` & `swibots-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.3.0
+Version: 1.3.1
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.3.0/README.md` & `swibots-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/setup.py` & `swibots-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = pypandoc.convert_file("README.md", "rst")
 except (IOError, ImportError):
     long_description = open("README.md").read()
 
 
 setup(
     name="swibots",
-    version="1.3.0",
+    version="1.3.1",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/switchcollab/Switch-Bots-Python-Library",
     description="Switch bot api",
     author="switchadmin",
     author_email="support@switch.pe",
```

### Comparing `swibots-1.3.0/swibots/api/api_client.py` & `swibots-1.3.1/swibots/api/api_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/auth/auth_client.py` & `swibots-1.3.1/swibots/api/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/auth/controllers/user_controller.py` & `swibots-1.3.1/swibots/api/auth/controllers/user_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ..models import AuthUser
 
 if TYPE_CHECKING:
     from swibots.api.auth import AuthClient
 
 log = logging.getLogger(__name__)
 
-BASE_PATH = "/user"
+BASE_PATH = "/api/user"
 T = TypeVar("T", bound="AuthUser")
 
 
 class UserController:
     """User controller
 
     This controller is used to communicate with the user endpoints.
```

### Comparing `swibots-1.3.0/swibots/api/auth/methods/get_me.py` & `swibots-1.3.1/swibots/api/auth/methods/get_me.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/auth/methods/login.py` & `swibots-1.3.1/swibots/api/auth/methods/login.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/auth/models/auth_user.py` & `swibots-1.3.1/swibots/api/auth/models/auth_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/bot/bot_client.py` & `swibots-1.3.1/swibots/api/bot/bot_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/bot/controllers/bot_controller.py` & `swibots-1.3.1/swibots/api/bot/controllers/bot_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/bot/methods/delete_bot_info.py` & `swibots-1.3.1/swibots/api/bot/methods/delete_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/bot/methods/get_bot_info.py` & `swibots-1.3.1/swibots/api/bot/methods/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/bot/methods/update_bot_info.py` & `swibots-1.3.1/swibots/api/bot/methods/update_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/bot/models/bot_command_info.py` & `swibots-1.3.1/swibots/api/bot/models/bot_command_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/bot/models/bot_info.py` & `swibots-1.3.1/swibots/api/bot/models/bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/chat_client.py` & `swibots-1.3.1/swibots/api/chat/chat_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/controllers/message_controller.py` & `swibots-1.3.1/swibots/api/chat/controllers/message_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/events/callback_query_event.py` & `swibots-1.3.1/swibots/api/chat/events/callback_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/events/chat_event.py` & `swibots-1.3.1/swibots/api/chat/events/chat_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/events/command_event.py` & `swibots-1.3.1/swibots/api/chat/events/command_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/events/inline_query_event.py` & `swibots-1.3.1/swibots/api/chat/events/inline_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/events/message_event.py` & `swibots-1.3.1/swibots/api/chat/events/message_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/__init__.py` & `swibots-1.3.1/swibots/api/chat/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/answer_inline_query.py` & `swibots-1.3.1/swibots/api/chat/methods/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/clear_conversation.py` & `swibots-1.3.1/swibots/api/chat/methods/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/delete_message.py` & `swibots-1.3.1/swibots/api/chat/methods/delete_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/delete_messages_from_user.py` & `swibots-1.3.1/swibots/api/chat/methods/delete_messages_from_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/download_media.py` & `swibots-1.3.1/swibots/api/chat/methods/download_media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/edit_message.py` & `swibots-1.3.1/swibots/api/chat/methods/edit_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/edit_message_text.py` & `swibots-1.3.1/swibots/api/chat/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/flag_message.py` & `swibots-1.3.1/swibots/api/chat/methods/flag_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/forward_message.py` & `swibots-1.3.1/swibots/api/chat/methods/forward_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/get_channel_chat_history.py` & `swibots-1.3.1/swibots/api/chat/methods/get_channel_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/get_community_media_files.py` & `swibots-1.3.1/swibots/api/chat/methods/get_community_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/get_community_media_files_by_status.py` & `swibots-1.3.1/swibots/api/chat/methods/get_community_media_files_by_status.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/get_flag_messages.py` & `swibots-1.3.1/swibots/api/chat/methods/get_flag_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/get_group_chat_history.py` & `swibots-1.3.1/swibots/api/chat/methods/get_group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/get_message.py` & `swibots-1.3.1/swibots/api/chat/methods/get_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/get_messages.py` & `swibots-1.3.1/swibots/api/chat/methods/get_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/get_messages_between_users.py` & `swibots-1.3.1/swibots/api/chat/methods/get_messages_between_users.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/get_unread_messages_count.py` & `swibots-1.3.1/swibots/api/chat/methods/get_unread_messages_count.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/get_user_media_files.py` & `swibots-1.3.1/swibots/api/chat/methods/get_user_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/reply_message.py` & `swibots-1.3.1/swibots/api/chat/methods/reply_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/reply_message_text.py` & `swibots-1.3.1/swibots/api/chat/methods/reply_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/send_message.py` & `swibots-1.3.1/swibots/api/chat/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/methods/send_text.py` & `swibots-1.3.1/swibots/api/chat/methods/send_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/group_chat_history.py` & `swibots-1.3.1/swibots/api/chat/models/group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline/__init__.py` & `swibots-1.3.1/swibots/api/chat/models/inline/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline/base_typed_inline_query_result.py` & `swibots-1.3.1/swibots/api/chat/models/inline/base_typed_inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline/inline_query.py` & `swibots-1.3.1/swibots/api/chat/models/inline/inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline/inline_query_answer.py` & `swibots-1.3.1/swibots/api/chat/models/inline/inline_query_answer.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline/inline_query_result.py` & `swibots-1.3.1/swibots/api/chat/models/inline/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline/inline_query_result_article.py` & `swibots-1.3.1/swibots/api/chat/models/inline/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline/inline_query_result_document.py` & `swibots-1.3.1/swibots/api/chat/models/inline/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline/inline_query_result_photo.py` & `swibots-1.3.1/swibots/api/chat/models/inline/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline/inline_query_result_video.py` & `swibots-1.3.1/swibots/api/chat/models/inline/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline/input_message_content.py` & `swibots-1.3.1/swibots/api/chat/models/inline/input_message_content.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline_keyboard_button.py` & `swibots-1.3.1/swibots/api/chat/models/inline_keyboard_button.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-from typing import List, Optional
+from typing import Optional
 
-import swibots
 from swibots.base import SwitchObject
-
 from swibots.utils.types import JSONDict
 
 
 class InlineKeyboardButton(SwitchObject):
     def __init__(
         self,
         text: Optional[str] = None,
         url: Optional[str] = None,
-        callback_data: Optional[str] = None,
+        callback_data: Optional[str] = None
     ):
         super().__init__(None)
         self.text = text
         self.url = url
         self.callback_data = callback_data
 
     def to_json(self) -> JSONDict:
         return {
             "text": self.text,
             "url": self.url,
-            "callbackData": self.callback_data,
+            "callbackData": self.callback_data
         }
 
     def from_json(self, data: JSONDict) -> "InlineKeyboardButton":
         if data is not None:
-            self.text = (data.get("text"),)
-            self.url = (data.get("url"),)
-            self.callback_data = (data.get("callbackData"),)
+            self.text = data.get("text")
+            self.url = data.get("url")
+            self.callback_data = data.get("callbackData")
         return self
```

### Comparing `swibots-1.3.0/swibots/api/chat/models/inline_markup.py` & `swibots-1.3.1/swibots/api/chat/models/inline_markup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import TYPE_CHECKING, List, Optional
-import swibots
-from .inline_keyboard_color import InlineKeyboardColor
-from .inline_keyboard_size import InlineKeyboardSize
-from .inline_keyboard_button import InlineKeyboardButton
-from swibots.base import SwitchObject
 
+from swibots.base import SwitchObject
 from swibots.utils.types import JSONDict
 
+from .inline_keyboard_button import InlineKeyboardButton
+from .inline_keyboard_color import InlineKeyboardColor
+from .inline_keyboard_size import InlineKeyboardSize
+
 if TYPE_CHECKING:
     from .inline_keyboard_button import InlineKeyboardButton
 
 
 class InlineMarkup(SwitchObject):
     def __init__(
         self,
@@ -29,15 +29,15 @@
             self._inline_keyboard = []
         return self._inline_keyboard
 
     def add_row(self, buttons: List["InlineKeyboardButton"]):
         if len(buttons) > 0:
             self.inline_keyboard.append(list(buttons))
 
-    def to_json(self) -> JSONDict:
+    def to_json(self) -> JSONDict | None:
         if self._inline_keyboard is None:
             return None
         return {
             "inlineKeyboard": [[x.to_json() for x in row] for row in self._inline_keyboard],
             "color": self._color.value,
             "size": self._size.value,
         }
@@ -58,20 +58,13 @@
                 form_data[url_key] = b.url
                 callback_data_key = 'inlineKeyboard.inlineKeyboard[{0}][{1}].callbackData'\
                     .format(i, j)
                 form_data[callback_data_key] = b.callback_data
         return form_data
 
     def from_json(self, data: JSONDict) -> "InlineMarkup":
-        if data is None or data.get("inlineKeyboard") is None:
-            return None
-        self._color = InlineKeyboardColor(data.get("color") or "RANDOM")
-        self._size = InlineKeyboardSize(data.get("size") or "DEFAULT")
-        self._inline_keyboard = (
-            [
-                [InlineKeyboardButton.build_from_json(
-                    x, self.app) for x in row]
-                for row in data.get("inlineKeyboard") or []
-            ],
-        )
-
+        if data is not None and data.get("inlineKeyboard") is not None:
+            self._color = InlineKeyboardColor(data.get("color") or "RANDOM")
+            self._size = InlineKeyboardSize(data.get("size") or "DEFAULT")
+            self._inline_keyboard = [[InlineKeyboardButton.build_from_json(x, self.app) for x in row]
+                                     for row in data.get("inlineKeyboard") or []]
         return self
```

### Comparing `swibots-1.3.0/swibots/api/chat/models/message.py` & `swibots-1.3.1/swibots/api/chat/models/message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/common/events/event.py` & `swibots-1.3.1/swibots/api/common/events/event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/common/models/media.py` & `swibots-1.3.1/swibots/api/common/models/media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/common/models/media_upload_request.py` & `swibots-1.3.1/swibots/api/common/models/media_upload_request.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/common/models/user.py` & `swibots-1.3.1/swibots/api/common/models/user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/community_client.py` & `swibots-1.3.1/swibots/api/community/community_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/controllers/channel_controller.py` & `swibots-1.3.1/swibots/api/community/controllers/channel_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/controllers/community_controller.py` & `swibots-1.3.1/swibots/api/community/controllers/community_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/controllers/group_controller.py` & `swibots-1.3.1/swibots/api/community/controllers/group_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/__init__.py` & `swibots-1.3.1/swibots/api/community/events/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/channel_created_event.py` & `swibots-1.3.1/swibots/api/community/events/channel_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/channel_deleted_event.py` & `swibots-1.3.1/swibots/api/community/events/channel_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/channel_updated_event.py` & `swibots-1.3.1/swibots/api/community/events/channel_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/community_event.py` & `swibots-1.3.1/swibots/api/community/events/community_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/community_updated_event.py` & `swibots-1.3.1/swibots/api/community/events/community_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/group_created_event.py` & `swibots-1.3.1/swibots/api/community/events/group_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/group_deleted_event.py` & `swibots-1.3.1/swibots/api/community/events/group_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/group_updated_event.py` & `swibots-1.3.1/swibots/api/community/events/group_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/member_joined_event.py` & `swibots-1.3.1/swibots/api/community/events/member_joined_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/member_left_event.py` & `swibots-1.3.1/swibots/api/community/events/member_left_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/events/user_banned_event.py` & `swibots-1.3.1/swibots/api/community/events/user_banned_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/methods/get_channel.py` & `swibots-1.3.1/swibots/api/community/methods/get_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/methods/get_community.py` & `swibots-1.3.1/swibots/api/community/methods/get_community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/methods/get_group.py` & `swibots-1.3.1/swibots/api/community/methods/get_group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/models/channel.py` & `swibots-1.3.1/swibots/api/community/models/channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/models/community.py` & `swibots-1.3.1/swibots/api/community/models/community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/api/community/models/group.py` & `swibots-1.3.1/swibots/api/community/models/group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/app.py` & `swibots-1.3.1/swibots/app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/base/rest_response.py` & `swibots-1.3.1/swibots/base/rest_response.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/base/switch_client.py` & `swibots-1.3.1/swibots/base/switch_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/base/switch_object.py` & `swibots-1.3.1/swibots/base/switch_object.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/base/switch_ws_async_client.py` & `swibots-1.3.1/swibots/base/switch_ws_async_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bot_app.py` & `swibots-1.3.1/swibots/bot_app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/bot.py` & `swibots-1.3.1/swibots/bots/bot.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/bot_context.py` & `swibots-1.3.1/swibots/bots/bot_context.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/__init__.py` & `swibots-1.3.1/swibots/bots/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_callback_query.py` & `swibots-1.3.1/swibots/bots/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_channel_created.py` & `swibots-1.3.1/swibots/bots/decorators/on_channel_created.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_channel_deleted.py` & `swibots-1.3.1/swibots/bots/decorators/on_channel_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_channel_updated.py` & `swibots-1.3.1/swibots/bots/decorators/on_channel_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_command.py` & `swibots-1.3.1/swibots/bots/decorators/on_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_community_updated.py` & `swibots-1.3.1/swibots/bots/decorators/on_community_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_group_created.py` & `swibots-1.3.1/swibots/bots/decorators/on_group_created.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_group_deleted.py` & `swibots-1.3.1/swibots/bots/decorators/on_group_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_group_updated.py` & `swibots-1.3.1/swibots/bots/decorators/on_group_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_inline_query.py` & `swibots-1.3.1/swibots/bots/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_member_joined.py` & `swibots-1.3.1/swibots/bots/decorators/on_member_joined.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_member_left.py` & `swibots-1.3.1/swibots/bots/decorators/on_member_left.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_message.py` & `swibots-1.3.1/swibots/bots/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_unknown_command.py` & `swibots-1.3.1/swibots/bots/decorators/on_unknown_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/decorators/on_user_banned.py` & `swibots-1.3.1/swibots/bots/decorators/on_user_banned.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/filters/filter.py` & `swibots-1.3.1/swibots/bots/filters/filter.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/__init__.py` & `swibots-1.3.1/swibots/bots/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/base_handler.py` & `swibots-1.3.1/swibots/bots/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/callback_query_handler.py` & `swibots-1.3.1/swibots/bots/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/channel_created_handler.py` & `swibots-1.3.1/swibots/bots/handlers/channel_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/channel_deleted_handler.py` & `swibots-1.3.1/swibots/bots/handlers/channel_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/channel_updated_handler.py` & `swibots-1.3.1/swibots/bots/handlers/channel_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/command_handler.py` & `swibots-1.3.1/swibots/bots/handlers/command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/community_updated_handler.py` & `swibots-1.3.1/swibots/bots/handlers/community_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/event_handler.py` & `swibots-1.3.1/swibots/bots/handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/group_created_handler.py` & `swibots-1.3.1/swibots/bots/handlers/group_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/group_deleted_handler.py` & `swibots-1.3.1/swibots/bots/handlers/group_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/group_updated_handler.py` & `swibots-1.3.1/swibots/bots/handlers/group_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/inline_query_handler.py` & `swibots-1.3.1/swibots/bots/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/member_joined_handler.py` & `swibots-1.3.1/swibots/bots/handlers/member_joined_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/member_left_handler.py` & `swibots-1.3.1/swibots/bots/handlers/member_left_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/message_handler.py` & `swibots-1.3.1/swibots/bots/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/unknown_command_handler.py` & `swibots-1.3.1/swibots/bots/handlers/unknown_command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/bots/handlers/user_banned_handler.py` & `swibots-1.3.1/swibots/bots/handlers/user_banned_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/config.py` & `swibots-1.3.1/swibots/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import os
 
 
 APP_CONFIG = {
     "CHAT_SERVICE": {
         "BASE_URL": os.getenv("CHAT_SERVICE_BASE_URL") or "https://chat.switch.pe",
-        "WS_URL": os.getenv("CHAT_SERVICE_WS_URL")
-        or "wss://api-gateway.switch.pe/v1/websocket/message/ws",
+        "WS_URL": os.getenv("CHAT_SERVICE_WS_URL") or "wss://chat.switch.pe/v1/websocket/message/ws",
     },
     "BOT_SERVICE": {
         "BASE_URL": os.getenv("BOT_SERVICE_BASE_URL") or "https://chat.switch.pe",
     },
     "AUTH_SERVICE": {
-        "BASE_URL": os.getenv("AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api",
+        "BASE_URL": os.getenv("AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/user-service",
     },
     "COMMUNITY_SERVICE": {
-        "BASE_URL": os.getenv("COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
-        "WS_URL": os.getenv("COMMUNITY_SERVICE_WS_URL")
-        or "wss://api-gateway.switch.pe/v1/websocket/community/ws",
+        "BASE_URL": os.getenv("COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/community-service",
+        "WS_URL": os.getenv("COMMUNITY_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/community/ws",
     },
 }
 
 
 def get_config():
     return APP_CONFIG
 
 
 def reload_config():
     APP_CONFIG["CHAT_SERVICE"]['BASE_URL'] = os.getenv(
         "CHAT_SERVICE_BASE_URL") or "https://chat.switch.pe"
     APP_CONFIG["CHAT_SERVICE"]['WS_URL'] = os.getenv(
-        "CHAT_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/message/ws"
+        "CHAT_SERVICE_WS_URL") or "wss://chat.switch.pe/v1/websocket/message/ws"
     APP_CONFIG["BOT_SERVICE"]['BASE_URL'] = os.getenv(
         "BOT_SERVICE_BASE_URL") or "https://chat.switch.pe"
     APP_CONFIG["AUTH_SERVICE"]['BASE_URL'] = os.getenv(
-        "AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api"
+        "AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/user-service"
     APP_CONFIG["COMMUNITY_SERVICE"]['BASE_URL'] = os.getenv(
-        "COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe"
+        "COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/community-service"
     APP_CONFIG["COMMUNITY_SERVICE"]['WS_URL'] = os.getenv(
         "COMMUNITY_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/community/ws"
 
 
 reload_config()
```

### Comparing `swibots-1.3.0/swibots/error.py` & `swibots-1.3.1/swibots/error.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/types.py` & `swibots-1.3.1/swibots/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/utils/rest_client.py` & `swibots-1.3.1/swibots/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/utils/types.py` & `swibots-1.3.1/swibots/utils/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/utils/ws/asyncstomp/async_ws_client.py` & `swibots-1.3.1/swibots/utils/ws/asyncstomp/async_ws_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/utils/ws/asyncstomp/async_ws_subscription.py` & `swibots-1.3.1/swibots/utils/ws/asyncstomp/async_ws_subscription.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots/utils/ws/common/ws_frame.py` & `swibots-1.3.1/swibots/utils/ws/common/ws_frame.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.0/swibots.egg-info/PKG-INFO` & `swibots-1.3.1/swibots.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.3.0
+Version: 1.3.1
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.3.0/swibots.egg-info/SOURCES.txt` & `swibots-1.3.1/swibots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

