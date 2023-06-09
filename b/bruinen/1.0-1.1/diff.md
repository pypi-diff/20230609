# Comparing `tmp/bruinen-1.0.tar.gz` & `tmp/bruinen-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bruinen-1.0.tar", max compression
+gzip compressed data, was "bruinen-1.1.tar", max compression
```

## Comparing `bruinen-1.0.tar` & `bruinen-1.1.tar`

### file list

```diff
@@ -1,199 +1,222 @@
--rw-r--r--   0        0        0     3789 2023-05-29 17:07:17.075681 bruinen-1.0/README.md
--rw-r--r--   0        0        0      559 2023-05-29 17:07:17.076269 bruinen-1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.076402 bruinen-1.0/src/bruinen/__init__.py
--rw-r--r--   0        0        0      155 2023-05-29 17:07:17.076603 bruinen-1.0/src/bruinen/client/__init__.py
--rw-r--r--   0        0        0       47 2023-05-29 17:07:17.076745 bruinen-1.0/src/bruinen/client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.076829 bruinen-1.0/src/bruinen/client/api/accounts/__init__.py
--rw-r--r--   0        0        0     2659 2023-06-04 18:35:15.594948 bruinen-1.0/src/bruinen/client/api/accounts/account_counts_for_policy.py
--rw-r--r--   0        0        0     3992 2023-05-29 17:07:17.077137 bruinen-1.0/src/bruinen/client/api/accounts/accounts_controller_deactivate.py
--rw-r--r--   0        0        0     4074 2023-05-29 17:07:17.077393 bruinen-1.0/src/bruinen/client/api/accounts/accounts_controller_get_accounts.py
--rw-r--r--   0        0        0     4080 2023-05-29 17:07:17.077523 bruinen-1.0/src/bruinen/client/api/accounts/find_all_accounts_for_user.py
--rw-r--r--   0        0        0     4087 2023-06-04 18:35:15.595026 bruinen-1.0/src/bruinen/client/api/accounts/find_all_active_for_user.py
--rw-r--r--   0        0        0     4094 2023-06-04 18:35:15.595086 bruinen-1.0/src/bruinen/client/api/accounts/find_all_active_with_policy_for_user.py
--rw-r--r--   0        0        0     3704 2023-05-29 17:07:17.077647 bruinen-1.0/src/bruinen/client/api/accounts/get_account.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.077737 bruinen-1.0/src/bruinen/client/api/auth/__init__.py
--rw-r--r--   0        0        0     3614 2023-05-29 17:07:17.077921 bruinen-1.0/src/bruinen/client/api/auth/get_user_auth_token.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.077997 bruinen-1.0/src/bruinen/client/api/confirm/__init__.py
--rw-r--r--   0        0        0     4144 2023-05-29 17:07:17.078189 bruinen-1.0/src/bruinen/client/api/confirm/create.py
--rw-r--r--   0        0        0     3703 2023-05-29 17:07:17.078301 bruinen-1.0/src/bruinen/client/api/confirm/find_one.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.078377 bruinen-1.0/src/bruinen/client/api/connection_requests/__init__.py
--rw-r--r--   0        0        0     4173 2023-05-29 17:07:17.078660 bruinen-1.0/src/bruinen/client/api/connection_requests/connection_requests_controller_find_all.py
--rw-r--r--   0        0        0     4319 2023-05-29 17:07:17.078777 bruinen-1.0/src/bruinen/client/api/connection_requests/create.py
--rw-r--r--   0        0        0     3668 2023-05-29 17:07:17.079084 bruinen-1.0/src/bruinen/client/api/connection_requests/get.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.079208 bruinen-1.0/src/bruinen/client/api/default/__init__.py
--rw-r--r--   0        0        0     3213 2023-05-29 17:07:17.079416 bruinen-1.0/src/bruinen/client/api/default/app_controller_get_hello.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.079525 bruinen-1.0/src/bruinen/client/api/source_policy/__init__.py
--rw-r--r--   0        0        0     3788 2023-05-29 17:07:17.079942 bruinen-1.0/src/bruinen/client/api/source_policy/source_policy_controller_deactivate.py
--rw-r--r--   0        0        0     3791 2023-05-29 17:07:17.080156 bruinen-1.0/src/bruinen/client/api/source_policy/source_policy_controller_get_all_active_for_client.py
--rw-r--r--   0        0        0     3800 2023-05-29 17:07:17.080418 bruinen-1.0/src/bruinen/client/api/source_policy/source_policy_controller_get_defaults_for_client.py
--rw-r--r--   0        0        0     3780 2023-05-29 17:07:17.080698 bruinen-1.0/src/bruinen/client/api/source_policy/source_policy_controller_get_policy_by_id.py
--rw-r--r--   0        0        0     3785 2023-05-29 17:07:17.080865 bruinen-1.0/src/bruinen/client/api/source_policy/source_policy_controller_set_default.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.080960 bruinen-1.0/src/bruinen/client/api/sources/__init__.py
--rw-r--r--   0        0        0     2356 2023-05-29 17:07:17.081261 bruinen-1.0/src/bruinen/client/api/sources/github_controller_get_auth_callback.py
--rw-r--r--   0        0        0     3963 2023-05-29 17:07:17.081512 bruinen-1.0/src/bruinen/client/api/sources/github_controller_profile.py
--rw-r--r--   0        0        0     4195 2023-06-04 18:35:15.595215 bruinen-1.0/src/bruinen/client/api/sources/github_controller_repos.py
--rw-r--r--   0        0        0     4371 2023-06-07 20:39:21.028826 bruinen-1.0/src/bruinen/client/api/sources/google_controller_calendar.py
--rw-r--r--   0        0        0     6460 2023-06-07 20:39:21.029215 bruinen-1.0/src/bruinen/client/api/sources/google_controller_calendars.py
--rw-r--r--   0        0        0     4272 2023-06-07 20:39:21.029544 bruinen-1.0/src/bruinen/client/api/sources/google_controller_draft.py
--rw-r--r--   0        0        0     4983 2023-06-07 20:39:21.029847 bruinen-1.0/src/bruinen/client/api/sources/google_controller_drafts.py
--rw-r--r--   0        0        0     5256 2023-06-07 20:39:21.030125 bruinen-1.0/src/bruinen/client/api/sources/google_controller_event.py
--rw-r--r--   0        0        0    11601 2023-06-07 20:39:21.030409 bruinen-1.0/src/bruinen/client/api/sources/google_controller_events.py
--rw-r--r--   0        0        0     2356 2023-06-04 18:35:15.595653 bruinen-1.0/src/bruinen/client/api/sources/google_controller_get_auth_callback.py
--rw-r--r--   0        0        0     4272 2023-06-07 20:39:21.030673 bruinen-1.0/src/bruinen/client/api/sources/google_controller_label.py
--rw-r--r--   0        0        0     3949 2023-06-04 18:35:15.595763 bruinen-1.0/src/bruinen/client/api/sources/google_controller_labels.py
--rw-r--r--   0        0        0     4338 2023-06-07 20:39:21.030934 bruinen-1.0/src/bruinen/client/api/sources/google_controller_message.py
--rw-r--r--   0        0        0     5587 2023-06-07 20:39:21.031174 bruinen-1.0/src/bruinen/client/api/sources/google_controller_messages.py
--rw-r--r--   0        0        0     3963 2023-06-04 18:35:15.595944 bruinen-1.0/src/bruinen/client/api/sources/google_controller_profile.py
--rw-r--r--   0        0        0     4305 2023-06-07 20:39:21.031429 bruinen-1.0/src/bruinen/client/api/sources/google_controller_thread.py
--rw-r--r--   0        0        0     5573 2023-06-07 20:39:21.031690 bruinen-1.0/src/bruinen/client/api/sources/google_controller_threads.py
--rw-r--r--   0        0        0     2349 2023-05-29 17:07:17.081920 bruinen-1.0/src/bruinen/client/api/sources/sources_controller_get_metadata.py
--rw-r--r--   0        0        0     4208 2023-05-29 17:07:17.082167 bruinen-1.0/src/bruinen/client/api/sources/sources_controller_get_metadata_for_source.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.082273 bruinen-1.0/src/bruinen/client/api/usage/__init__.py
--rw-r--r--   0        0        0     3984 2023-05-29 17:07:17.082481 bruinen-1.0/src/bruinen/client/api/usage/usage_controller_find_all.py
--rw-r--r--   0        0        0     2482 2023-05-29 17:07:17.082610 bruinen-1.0/src/bruinen/client/api/usage/usage_controller_find_one.py
--rw-r--r--   0        0        0     3417 2023-05-29 17:07:17.082739 bruinen-1.0/src/bruinen/client/api/usage/usage_controller_get_client_data.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.082838 bruinen-1.0/src/bruinen/client/api/users/__init__.py
--rw-r--r--   0        0        0     3991 2023-05-29 17:07:17.083019 bruinen-1.0/src/bruinen/client/api/users/users_controller_create.py
--rw-r--r--   0        0        0     3682 2023-05-29 17:07:17.083145 bruinen-1.0/src/bruinen/client/api/users/users_controller_find_all.py
--rw-r--r--   0        0        0     3667 2023-05-29 17:07:17.083272 bruinen-1.0/src/bruinen/client/api/users/users_controller_find_one.py
--rw-r--r--   0        0        0     3405 2023-05-29 17:07:17.083393 bruinen-1.0/src/bruinen/client/api/users/users_controller_find_user_from_token.py
--rw-r--r--   0        0        0     4200 2023-05-29 17:07:17.083516 bruinen-1.0/src/bruinen/client/api/users/users_controller_update.py
--rw-r--r--   0        0        0     3998 2023-05-29 17:07:17.083732 bruinen-1.0/src/bruinen/client/api/users/users_controller_upsert_user.py
--rw-r--r--   0        0        0     2817 2023-05-29 17:07:17.083845 bruinen-1.0/src/bruinen/client/client.py
--rw-r--r--   0        0        0      470 2023-05-29 17:07:17.083960 bruinen-1.0/src/bruinen/client/errors.py
--rw-r--r--   0        0        0    14209 2023-06-07 20:39:21.031957 bruinen-1.0/src/bruinen/client/models/__init__.py
--rw-r--r--   0        0        0      214 2023-05-29 17:07:17.084256 bruinen-1.0/src/bruinen/client/models/account_status.py
--rw-r--r--   0        0        0     1296 2023-05-29 17:07:17.084513 bruinen-1.0/src/bruinen/client/models/accounts_controller_deactivate_response_200.py
--rw-r--r--   0        0        0     1327 2023-05-29 17:07:17.084754 bruinen-1.0/src/bruinen/client/models/accounts_controller_get_accounts_response_200_item.py
--rw-r--r--   0        0        0     1394 2023-05-29 17:07:17.084879 bruinen-1.0/src/bruinen/client/models/auth.py
--rw-r--r--   0        0        0     2933 2023-05-29 17:07:17.085003 bruinen-1.0/src/bruinen/client/models/client_usage_data.py
--rw-r--r--   0        0        0      245 2023-05-29 17:07:17.085117 bruinen-1.0/src/bruinen/client/models/confirmation_status.py
--rw-r--r--   0        0        0     1360 2023-05-29 17:07:17.085263 bruinen-1.0/src/bruinen/client/models/connection_requests_controller_find_all_response_200_item.py
--rw-r--r--   0        0        0     3000 2023-05-29 17:07:17.085387 bruinen-1.0/src/bruinen/client/models/create_confirm_dto.py
--rw-r--r--   0        0        0     1208 2023-05-29 17:07:17.085492 bruinen-1.0/src/bruinen/client/models/create_confirm_dto_params.py
--rw-r--r--   0        0        0     2064 2023-05-29 17:07:17.085596 bruinen-1.0/src/bruinen/client/models/create_confirm_returned_dto.py
--rw-r--r--   0        0        0     2988 2023-05-29 17:07:17.085708 bruinen-1.0/src/bruinen/client/models/create_connection_request_dto.py
--rw-r--r--   0        0        0     1261 2023-05-29 17:07:17.085820 bruinen-1.0/src/bruinen/client/models/create_connection_request_dto_source.py
--rw-r--r--   0        0        0     2362 2023-05-29 17:07:17.085952 bruinen-1.0/src/bruinen/client/models/create_user_dto.py
--rw-r--r--   0        0        0      193 2023-05-29 17:07:17.086253 bruinen-1.0/src/bruinen/client/models/credential_provider.py
--rw-r--r--   0        0        0     2141 2023-05-29 17:07:17.086421 bruinen-1.0/src/bruinen/client/models/endpoint_data.py
--rw-r--r--   0        0        0     1165 2023-05-29 17:07:17.086580 bruinen-1.0/src/bruinen/client/models/get_response_200.py
--rw-r--r--   0        0        0    13880 2023-05-29 17:07:17.086746 bruinen-1.0/src/bruinen/client/models/github_profile.py
--rw-r--r--   0        0        0    27798 2023-05-29 17:07:17.087060 bruinen-1.0/src/bruinen/client/models/github_repo.py
--rw-r--r--   0        0        0    13906 2023-05-29 17:07:17.087227 bruinen-1.0/src/bruinen/client/models/github_repo_owner.py
--rw-r--r--   0        0        0     2751 2023-05-29 17:07:17.087375 bruinen-1.0/src/bruinen/client/models/github_repo_permissions.py
--rw-r--r--   0        0        0     4464 2023-06-04 18:35:15.596297 bruinen-1.0/src/bruinen/client/models/google_calendar.py
--rw-r--r--   0        0        0     2188 2023-06-04 18:35:15.596970 bruinen-1.0/src/bruinen/client/models/google_calendar_conference_properties.py
--rw-r--r--   0        0        0     3595 2023-06-04 18:35:15.597143 bruinen-1.0/src/bruinen/client/models/google_calendars.py
--rw-r--r--   0        0        0    10266 2023-06-04 18:35:15.597256 bruinen-1.0/src/bruinen/client/models/google_calendars_calendars_item.py
--rw-r--r--   0        0        0     2264 2023-06-04 18:35:15.597314 bruinen-1.0/src/bruinen/client/models/google_calendars_calendars_item_conference_properties.py
--rw-r--r--   0        0        0     2024 2023-06-04 18:35:15.597376 bruinen-1.0/src/bruinen/client/models/google_calendars_calendars_item_default_reminders.py
--rw-r--r--   0        0        0     3002 2023-06-04 18:35:15.597439 bruinen-1.0/src/bruinen/client/models/google_calendars_calendars_item_notification_settings.py
--rw-r--r--   0        0        0     2052 2023-06-04 18:35:15.597514 bruinen-1.0/src/bruinen/client/models/google_calendars_calendars_item_notification_settings_notifications_item.py
--rw-r--r--   0        0        0     2268 2023-06-04 18:35:15.597643 bruinen-1.0/src/bruinen/client/models/google_draft.py
--rw-r--r--   0        0        0     4723 2023-06-04 18:35:15.597766 bruinen-1.0/src/bruinen/client/models/google_draft_message.py
--rw-r--r--   0        0        0     5102 2023-06-04 18:35:15.597851 bruinen-1.0/src/bruinen/client/models/google_draft_message_payload.py
--rw-r--r--   0        0        0     2138 2023-06-04 18:35:15.597937 bruinen-1.0/src/bruinen/client/models/google_draft_message_payload_body.py
--rw-r--r--   0        0        0     1830 2023-06-04 18:35:15.598013 bruinen-1.0/src/bruinen/client/models/google_draft_message_payload_headers_item.py
--rw-r--r--   0        0        0     4311 2023-06-04 18:35:15.598093 bruinen-1.0/src/bruinen/client/models/google_draft_message_payload_parts_item.py
--rw-r--r--   0        0        0     2186 2023-06-04 18:35:15.598162 bruinen-1.0/src/bruinen/client/models/google_draft_message_payload_parts_item_body.py
--rw-r--r--   0        0        0     1881 2023-06-04 18:35:15.598224 bruinen-1.0/src/bruinen/client/models/google_draft_message_payload_parts_item_headers_item.py
--rw-r--r--   0        0        0     3038 2023-06-04 18:35:15.598701 bruinen-1.0/src/bruinen/client/models/google_drafts.py
--rw-r--r--   0        0        0     2403 2023-06-04 18:35:15.598773 bruinen-1.0/src/bruinen/client/models/google_drafts_drafts_item.py
--rw-r--r--   0        0        0     1887 2023-06-04 18:35:15.598854 bruinen-1.0/src/bruinen/client/models/google_drafts_drafts_item_message.py
--rw-r--r--   0        0        0    21058 2023-06-04 18:35:15.599019 bruinen-1.0/src/bruinen/client/models/google_event.py
--rw-r--r--   0        0        0     2812 2023-06-04 18:35:15.599103 bruinen-1.0/src/bruinen/client/models/google_event_attachments_item.py
--rw-r--r--   0        0        0     4469 2023-06-04 18:35:15.599171 bruinen-1.0/src/bruinen/client/models/google_event_attendees_item.py
--rw-r--r--   0        0        0     5871 2023-06-04 18:35:15.599240 bruinen-1.0/src/bruinen/client/models/google_event_conference_data.py
--rw-r--r--   0        0        0     3028 2023-06-04 18:35:15.599307 bruinen-1.0/src/bruinen/client/models/google_event_conference_data_conference_solution.py
--rw-r--r--   0        0        0     1694 2023-06-04 18:35:15.599366 bruinen-1.0/src/bruinen/client/models/google_event_conference_data_conference_solution_key.py
--rw-r--r--   0        0        0     4265 2023-06-04 18:35:15.599432 bruinen-1.0/src/bruinen/client/models/google_event_conference_data_create_request.py
--rw-r--r--   0        0        0     1796 2023-06-04 18:35:15.599487 bruinen-1.0/src/bruinen/client/models/google_event_conference_data_create_request_conference_solution_key.py
--rw-r--r--   0        0        0     1766 2023-06-04 18:35:15.599549 bruinen-1.0/src/bruinen/client/models/google_event_conference_data_create_request_status.py
--rw-r--r--   0        0        0     3860 2023-06-04 18:35:15.599619 bruinen-1.0/src/bruinen/client/models/google_event_conference_data_entry_points_item.py
--rw-r--r--   0        0        0     2401 2023-06-04 18:35:15.599685 bruinen-1.0/src/bruinen/client/models/google_event_creator.py
--rw-r--r--   0        0        0     2127 2023-06-04 18:35:15.599756 bruinen-1.0/src/bruinen/client/models/google_event_end.py
--rw-r--r--   0        0        0     3226 2023-06-04 18:35:15.599815 bruinen-1.0/src/bruinen/client/models/google_event_extended_properties.py
--rw-r--r--   0        0        0     1323 2023-06-04 18:35:15.599869 bruinen-1.0/src/bruinen/client/models/google_event_extended_properties_private.py
--rw-r--r--   0        0        0     1317 2023-06-04 18:35:15.599944 bruinen-1.0/src/bruinen/client/models/google_event_extended_properties_shared.py
--rw-r--r--   0        0        0     4170 2023-06-04 18:35:15.600008 bruinen-1.0/src/bruinen/client/models/google_event_gadget.py
--rw-r--r--   0        0        0     1266 2023-06-04 18:35:15.600065 bruinen-1.0/src/bruinen/client/models/google_event_gadget_preferences.py
--rw-r--r--   0        0        0     2421 2023-06-04 18:35:15.600189 bruinen-1.0/src/bruinen/client/models/google_event_organizer.py
--rw-r--r--   0        0        0     2259 2023-06-04 18:35:15.600242 bruinen-1.0/src/bruinen/client/models/google_event_original_start_time.py
--rw-r--r--   0        0        0     2753 2023-06-04 18:35:15.600338 bruinen-1.0/src/bruinen/client/models/google_event_reminders.py
--rw-r--r--   0        0        0     1953 2023-06-04 18:35:15.600402 bruinen-1.0/src/bruinen/client/models/google_event_reminders_overrides_item.py
--rw-r--r--   0        0        0     1785 2023-06-04 18:35:15.600454 bruinen-1.0/src/bruinen/client/models/google_event_source.py
--rw-r--r--   0        0        0     2145 2023-06-04 18:35:15.600508 bruinen-1.0/src/bruinen/client/models/google_event_start.py
--rw-r--r--   0        0        0     6772 2023-06-04 18:35:15.600564 bruinen-1.0/src/bruinen/client/models/google_events.py
--rw-r--r--   0        0        0     1924 2023-06-04 18:35:15.600615 bruinen-1.0/src/bruinen/client/models/google_events_default_reminders_item.py
--rw-r--r--   0        0        0    22193 2023-06-04 18:35:15.600676 bruinen-1.0/src/bruinen/client/models/google_events_events_item.py
--rw-r--r--   0        0        0     2873 2023-06-04 18:35:15.600743 bruinen-1.0/src/bruinen/client/models/google_events_events_item_attachments_item.py
--rw-r--r--   0        0        0     4530 2023-06-04 18:35:15.600796 bruinen-1.0/src/bruinen/client/models/google_events_events_item_attendees_item.py
--rw-r--r--   0        0        0     6310 2023-06-04 18:35:15.600848 bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data.py
--rw-r--r--   0        0        0     3181 2023-06-04 18:35:15.600903 bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution.py
--rw-r--r--   0        0        0     1755 2023-06-04 18:35:15.600953 bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution_key.py
--rw-r--r--   0        0        0     4541 2023-06-04 18:35:15.601008 bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_create_request.py
--rw-r--r--   0        0        0     1857 2023-06-04 18:35:15.601064 bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_create_request_conference_solution_key.py
--rw-r--r--   0        0        0     1827 2023-06-04 18:35:15.601123 bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_create_request_status.py
--rw-r--r--   0        0        0     3921 2023-06-04 18:35:15.601184 bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_entry_points_item.py
--rw-r--r--   0        0        0     2462 2023-06-04 18:35:15.601243 bruinen-1.0/src/bruinen/client/models/google_events_events_item_creator.py
--rw-r--r--   0        0        0     2188 2023-06-04 18:35:15.601300 bruinen-1.0/src/bruinen/client/models/google_events_events_item_end.py
--rw-r--r--   0        0        0     3579 2023-06-04 18:35:15.601359 bruinen-1.0/src/bruinen/client/models/google_events_events_item_extended_properties.py
--rw-r--r--   0        0        0     1384 2023-06-04 18:35:15.601415 bruinen-1.0/src/bruinen/client/models/google_events_events_item_extended_properties_private.py
--rw-r--r--   0        0        0     1378 2023-06-04 18:35:15.601467 bruinen-1.0/src/bruinen/client/models/google_events_events_item_extended_properties_shared.py
--rw-r--r--   0        0        0     4323 2023-06-04 18:35:15.601835 bruinen-1.0/src/bruinen/client/models/google_events_events_item_gadget.py
--rw-r--r--   0        0        0     1327 2023-06-04 18:35:15.601902 bruinen-1.0/src/bruinen/client/models/google_events_events_item_gadget_preferences.py
--rw-r--r--   0        0        0     2482 2023-06-04 18:35:15.601966 bruinen-1.0/src/bruinen/client/models/google_events_events_item_organizer.py
--rw-r--r--   0        0        0     2320 2023-06-04 18:35:15.602020 bruinen-1.0/src/bruinen/client/models/google_events_events_item_original_start_time.py
--rw-r--r--   0        0        0     2920 2023-06-04 18:35:15.602089 bruinen-1.0/src/bruinen/client/models/google_events_events_item_reminders.py
--rw-r--r--   0        0        0     2014 2023-06-04 18:35:15.602146 bruinen-1.0/src/bruinen/client/models/google_events_events_item_reminders_overrides_item.py
--rw-r--r--   0        0        0     1846 2023-06-04 18:35:15.602206 bruinen-1.0/src/bruinen/client/models/google_events_events_item_source.py
--rw-r--r--   0        0        0     2206 2023-06-04 18:35:15.602297 bruinen-1.0/src/bruinen/client/models/google_events_events_item_start.py
--rw-r--r--   0        0        0     5170 2023-06-04 18:35:15.602438 bruinen-1.0/src/bruinen/client/models/google_label.py
--rw-r--r--   0        0        0     1927 2023-06-04 18:35:15.602502 bruinen-1.0/src/bruinen/client/models/google_label_color.py
--rw-r--r--   0        0        0     2652 2023-06-04 18:35:15.602612 bruinen-1.0/src/bruinen/client/models/google_labels.py
--rw-r--r--   0        0        0     2945 2023-06-04 18:35:15.602671 bruinen-1.0/src/bruinen/client/models/google_labels_labels_item.py
--rw-r--r--   0        0        0     4411 2023-06-04 18:35:15.602731 bruinen-1.0/src/bruinen/client/models/google_message.py
--rw-r--r--   0        0        0     4958 2023-06-04 18:35:15.602891 bruinen-1.0/src/bruinen/client/models/google_message_payload.py
--rw-r--r--   0        0        0     2110 2023-06-04 18:35:15.602959 bruinen-1.0/src/bruinen/client/models/google_message_payload_body.py
--rw-r--r--   0        0        0     1802 2023-06-04 18:35:15.603022 bruinen-1.0/src/bruinen/client/models/google_message_payload_headers_item.py
--rw-r--r--   0        0        0     4162 2023-06-04 18:35:15.603092 bruinen-1.0/src/bruinen/client/models/google_message_payload_parts_item.py
--rw-r--r--   0        0        0     2158 2023-06-04 18:35:15.603148 bruinen-1.0/src/bruinen/client/models/google_message_payload_parts_item_body.py
--rw-r--r--   0        0        0     1853 2023-06-04 18:35:15.603215 bruinen-1.0/src/bruinen/client/models/google_message_payload_parts_item_headers_item.py
--rw-r--r--   0        0        0     3115 2023-06-04 18:35:15.603282 bruinen-1.0/src/bruinen/client/models/google_messages.py
--rw-r--r--   0        0        0     1844 2023-06-04 18:35:15.603404 bruinen-1.0/src/bruinen/client/models/google_messages_messages_item.py
--rw-r--r--   0        0        0     2662 2023-06-04 18:35:15.603466 bruinen-1.0/src/bruinen/client/models/google_profile.py
--rw-r--r--   0        0        0     3121 2023-06-04 18:35:15.603520 bruinen-1.0/src/bruinen/client/models/google_thread.py
--rw-r--r--   0        0        0     4544 2023-06-04 18:35:15.603635 bruinen-1.0/src/bruinen/client/models/google_thread_messages_item.py
--rw-r--r--   0        0        0     5273 2023-06-04 18:35:15.603690 bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload.py
--rw-r--r--   0        0        0     2171 2023-06-04 18:35:15.603744 bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload_body.py
--rw-r--r--   0        0        0     1863 2023-06-04 18:35:15.603804 bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload_headers_item.py
--rw-r--r--   0        0        0     4480 2023-06-04 18:35:15.603858 bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload_parts_item.py
--rw-r--r--   0        0        0     2219 2023-06-04 18:35:15.603914 bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_body.py
--rw-r--r--   0        0        0     1914 2023-06-04 18:35:15.603970 bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_headers_item.py
--rw-r--r--   0        0        0     3068 2023-06-04 18:35:15.604038 bruinen-1.0/src/bruinen/client/models/google_threads.py
--rw-r--r--   0        0        0     2135 2023-06-04 18:35:15.604149 bruinen-1.0/src/bruinen/client/models/google_threads_threads_item.py
--rw-r--r--   0        0        0     3499 2023-05-29 17:07:17.087500 bruinen-1.0/src/bruinen/client/models/returned_account_dto.py
--rw-r--r--   0        0        0     4714 2023-05-29 17:07:17.087618 bruinen-1.0/src/bruinen/client/models/returned_confirm_dto.py
--rw-r--r--   0        0        0     1218 2023-05-29 17:07:17.087719 bruinen-1.0/src/bruinen/client/models/returned_confirm_dto_params.py
--rw-r--r--   0        0        0     3613 2023-05-29 17:07:17.087832 bruinen-1.0/src/bruinen/client/models/returned_connection_request_dto.py
--rw-r--r--   0        0        0     1271 2023-05-29 17:07:17.087942 bruinen-1.0/src/bruinen/client/models/returned_connection_request_dto_source.py
--rw-r--r--   0        0        0     4313 2023-05-29 17:07:17.088240 bruinen-1.0/src/bruinen/client/models/returned_source_policy_dto.py
--rw-r--r--   0        0        0     2719 2023-05-29 17:07:17.088365 bruinen-1.0/src/bruinen/client/models/returned_user_dto.py
--rw-r--r--   0        0        0     2901 2023-05-29 17:07:17.088468 bruinen-1.0/src/bruinen/client/models/source_data.py
--rw-r--r--   0        0        0      177 2023-05-29 17:07:17.088684 bruinen-1.0/src/bruinen/client/models/source_policy_status.py
--rw-r--r--   0        0        0      549 2023-05-29 17:07:17.088783 bruinen-1.0/src/bruinen/client/models/source_type.py
--rw-r--r--   0        0        0     1350 2023-05-29 17:07:17.089063 bruinen-1.0/src/bruinen/client/models/sources_controller_get_metadata_for_source_response_200.py
--rw-r--r--   0        0        0     2362 2023-05-29 17:07:17.089219 bruinen-1.0/src/bruinen/client/models/update_user_dto.py
--rw-r--r--   0        0        0     2362 2023-05-29 17:07:17.089363 bruinen-1.0/src/bruinen/client/models/upsert_user_dto.py
--rw-r--r--   0        0        0     1292 2023-05-29 17:07:17.089481 bruinen-1.0/src/bruinen/client/models/usage_controller_find_all_response_200_item.py
--rw-r--r--   0        0        0       25 2023-05-29 17:07:17.089579 bruinen-1.0/src/bruinen/client/py.typed
--rw-r--r--   0        0        0      993 2023-05-29 17:07:17.089682 bruinen-1.0/src/bruinen/client/types.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.089753 bruinen-1.0/src/bruinen/confirm/__init__.py
--rw-r--r--   0        0        0     2032 2023-05-29 17:07:17.089933 bruinen-1.0/src/bruinen/confirm/confirm.py
--rw-r--r--   0        0        0        0 2023-05-29 17:07:17.090017 bruinen-1.0/src/bruinen/langchain/__init__.py
--rw-r--r--   0        0        0     6107 2023-06-07 20:39:21.032227 bruinen-1.0/src/bruinen/langchain/github.py
--rw-r--r--   0        0        0    49841 2023-06-07 20:39:21.032615 bruinen-1.0/src/bruinen/langchain/google.py
--rw-r--r--   0        0        0       34 2023-06-07 20:39:21.032868 bruinen-1.0/src/bruinen/langchain/parsers/__init__.py
--rw-r--r--   0        0        0     4683 2023-06-07 20:39:21.033189 bruinen-1.0/src/bruinen/langchain/parsers/sql_parser.py
--rw-r--r--   0        0        0     4330 1970-01-01 00:00:00.000000 bruinen-1.0/PKG-INFO
+-rw-r--r--   0        0        0      733 2023-06-09 17:43:51.803315 bruinen-1.1/README.md
+-rw-r--r--   0        0        0      559 2023-06-09 17:56:24.755885 bruinen-1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 21:25:54.158184 bruinen-1.1/src/bruinen/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-08 18:28:15.758566 bruinen-1.1/src/bruinen/client/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-08 18:28:14.056229 bruinen-1.1/src/bruinen/client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:28:14.076287 bruinen-1.1/src/bruinen/client/api/accounts/__init__.py
+-rw-r--r--   0        0        0     2659 2023-06-08 18:28:15.770523 bruinen-1.1/src/bruinen/client/api/accounts/account_counts_for_policy.py
+-rw-r--r--   0        0        0     3992 2023-06-08 18:28:15.796019 bruinen-1.1/src/bruinen/client/api/accounts/accounts_controller_deactivate.py
+-rw-r--r--   0        0        0     4074 2023-06-08 18:28:15.777083 bruinen-1.1/src/bruinen/client/api/accounts/accounts_controller_get_accounts.py
+-rw-r--r--   0        0        0     4080 2023-06-08 18:28:15.799474 bruinen-1.1/src/bruinen/client/api/accounts/find_all_accounts_for_user.py
+-rw-r--r--   0        0        0     4087 2023-06-08 18:28:15.794157 bruinen-1.1/src/bruinen/client/api/accounts/find_all_active_for_user.py
+-rw-r--r--   0        0        0     4094 2023-06-08 18:28:15.806544 bruinen-1.1/src/bruinen/client/api/accounts/find_all_active_with_policy_for_user.py
+-rw-r--r--   0        0        0     3704 2023-06-08 18:28:15.782638 bruinen-1.1/src/bruinen/client/api/accounts/get_account.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:28:14.078538 bruinen-1.1/src/bruinen/client/api/auth/__init__.py
+-rw-r--r--   0        0        0     3614 2023-06-08 18:28:15.779257 bruinen-1.1/src/bruinen/client/api/auth/get_user_auth_token.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:28:14.095346 bruinen-1.1/src/bruinen/client/api/confirm/__init__.py
+-rw-r--r--   0        0        0     4144 2023-06-08 18:28:15.789233 bruinen-1.1/src/bruinen/client/api/confirm/create.py
+-rw-r--r--   0        0        0     3703 2023-06-08 18:28:15.798171 bruinen-1.1/src/bruinen/client/api/confirm/find_one.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:28:14.078948 bruinen-1.1/src/bruinen/client/api/connection_requests/__init__.py
+-rw-r--r--   0        0        0     4173 2023-06-08 18:28:15.819241 bruinen-1.1/src/bruinen/client/api/connection_requests/connection_requests_controller_find_all.py
+-rw-r--r--   0        0        0     4319 2023-06-08 18:28:15.815398 bruinen-1.1/src/bruinen/client/api/connection_requests/create.py
+-rw-r--r--   0        0        0     3668 2023-06-08 18:28:15.817072 bruinen-1.1/src/bruinen/client/api/connection_requests/get.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:28:14.092898 bruinen-1.1/src/bruinen/client/api/source_policy/__init__.py
+-rw-r--r--   0        0        0     3791 2023-06-08 18:28:15.812952 bruinen-1.1/src/bruinen/client/api/source_policy/source_policy_controller_get_all_active_for_client.py
+-rw-r--r--   0        0        0     3800 2023-06-08 18:28:15.835433 bruinen-1.1/src/bruinen/client/api/source_policy/source_policy_controller_get_defaults_for_client.py
+-rw-r--r--   0        0        0     3780 2023-06-08 18:28:15.814810 bruinen-1.1/src/bruinen/client/api/source_policy/source_policy_controller_get_policy_by_id.py
+-rw-r--r--   0        0        0     3785 2023-06-08 18:28:15.822626 bruinen-1.1/src/bruinen/client/api/source_policy/source_policy_controller_set_default.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:28:14.080079 bruinen-1.1/src/bruinen/client/api/sources/__init__.py
+-rw-r--r--   0        0        0     3963 2023-06-08 18:28:15.848258 bruinen-1.1/src/bruinen/client/api/sources/github_controller_profile.py
+-rw-r--r--   0        0        0     4195 2023-06-08 18:28:15.836495 bruinen-1.1/src/bruinen/client/api/sources/github_controller_repos.py
+-rw-r--r--   0        0        0     4371 2023-06-08 18:28:15.895622 bruinen-1.1/src/bruinen/client/api/sources/google_controller_calendar.py
+-rw-r--r--   0        0        0     6460 2023-06-08 18:28:15.868203 bruinen-1.1/src/bruinen/client/api/sources/google_controller_calendars.py
+-rw-r--r--   0        0        0     4272 2023-06-08 18:28:15.870787 bruinen-1.1/src/bruinen/client/api/sources/google_controller_draft.py
+-rw-r--r--   0        0        0     4983 2023-06-08 18:28:15.864435 bruinen-1.1/src/bruinen/client/api/sources/google_controller_drafts.py
+-rw-r--r--   0        0        0     5256 2023-06-08 18:28:15.870788 bruinen-1.1/src/bruinen/client/api/sources/google_controller_event.py
+-rw-r--r--   0        0        0    11601 2023-06-08 18:28:15.948526 bruinen-1.1/src/bruinen/client/api/sources/google_controller_events.py
+-rw-r--r--   0        0        0     4272 2023-06-08 18:28:15.895190 bruinen-1.1/src/bruinen/client/api/sources/google_controller_label.py
+-rw-r--r--   0        0        0     3949 2023-06-08 18:28:15.888002 bruinen-1.1/src/bruinen/client/api/sources/google_controller_labels.py
+-rw-r--r--   0        0        0     4338 2023-06-08 18:28:15.901114 bruinen-1.1/src/bruinen/client/api/sources/google_controller_message.py
+-rw-r--r--   0        0        0     5587 2023-06-08 18:28:15.916597 bruinen-1.1/src/bruinen/client/api/sources/google_controller_messages.py
+-rw-r--r--   0        0        0     4357 2023-06-09 17:40:25.901908 bruinen-1.1/src/bruinen/client/api/sources/google_controller_parsed_draft.py
+-rw-r--r--   0        0        0     4423 2023-06-09 17:40:25.902189 bruinen-1.1/src/bruinen/client/api/sources/google_controller_parsed_message.py
+-rw-r--r--   0        0        0     4390 2023-06-09 17:40:25.902542 bruinen-1.1/src/bruinen/client/api/sources/google_controller_parsed_thread.py
+-rw-r--r--   0        0        0     3963 2023-06-08 18:28:15.926648 bruinen-1.1/src/bruinen/client/api/sources/google_controller_profile.py
+-rw-r--r--   0        0        0     4305 2023-06-08 18:28:15.924378 bruinen-1.1/src/bruinen/client/api/sources/google_controller_thread.py
+-rw-r--r--   0        0        0     5573 2023-06-08 18:28:15.950335 bruinen-1.1/src/bruinen/client/api/sources/google_controller_threads.py
+-rw-r--r--   0        0        0     2349 2023-06-08 18:28:15.930638 bruinen-1.1/src/bruinen/client/api/sources/sources_controller_get_metadata.py
+-rw-r--r--   0        0        0     4208 2023-06-08 18:28:15.945865 bruinen-1.1/src/bruinen/client/api/sources/sources_controller_get_metadata_for_source.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:28:14.092046 bruinen-1.1/src/bruinen/client/api/usage/__init__.py
+-rw-r--r--   0        0        0     3984 2023-06-08 18:28:15.968189 bruinen-1.1/src/bruinen/client/api/usage/usage_controller_find_all.py
+-rw-r--r--   0        0        0     2482 2023-06-08 18:28:15.955352 bruinen-1.1/src/bruinen/client/api/usage/usage_controller_find_one.py
+-rw-r--r--   0        0        0     3417 2023-06-08 18:28:15.957803 bruinen-1.1/src/bruinen/client/api/usage/usage_controller_get_client_data.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:28:14.062409 bruinen-1.1/src/bruinen/client/api/users/__init__.py
+-rw-r--r--   0        0        0     3991 2023-06-08 18:28:15.980628 bruinen-1.1/src/bruinen/client/api/users/users_controller_create.py
+-rw-r--r--   0        0        0     3682 2023-06-08 18:28:15.959935 bruinen-1.1/src/bruinen/client/api/users/users_controller_find_all.py
+-rw-r--r--   0        0        0     3667 2023-06-08 18:28:15.969913 bruinen-1.1/src/bruinen/client/api/users/users_controller_find_one.py
+-rw-r--r--   0        0        0     3405 2023-06-08 18:28:15.975994 bruinen-1.1/src/bruinen/client/api/users/users_controller_find_user_from_token.py
+-rw-r--r--   0        0        0     4200 2023-06-08 18:28:15.983542 bruinen-1.1/src/bruinen/client/api/users/users_controller_update.py
+-rw-r--r--   0        0        0     3998 2023-06-08 18:28:15.992367 bruinen-1.1/src/bruinen/client/api/users/users_controller_upsert_user.py
+-rw-r--r--   0        0        0     2817 2023-06-08 18:28:15.977532 bruinen-1.1/src/bruinen/client/client.py
+-rw-r--r--   0        0        0      470 2023-06-08 18:28:15.968530 bruinen-1.1/src/bruinen/client/errors.py
+-rw-r--r--   0        0        0    17446 2023-06-09 17:40:25.902790 bruinen-1.1/src/bruinen/client/models/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-08 18:28:14.873142 bruinen-1.1/src/bruinen/client/models/account_status.py
+-rw-r--r--   0        0        0     1296 2023-06-08 18:28:15.986989 bruinen-1.1/src/bruinen/client/models/accounts_controller_deactivate_response_200.py
+-rw-r--r--   0        0        0     1327 2023-06-08 18:28:15.978818 bruinen-1.1/src/bruinen/client/models/accounts_controller_get_accounts_response_200_item.py
+-rw-r--r--   0        0        0     1394 2023-06-08 18:28:15.995149 bruinen-1.1/src/bruinen/client/models/auth.py
+-rw-r--r--   0        0        0     2933 2023-06-08 18:28:16.031417 bruinen-1.1/src/bruinen/client/models/client_usage_data.py
+-rw-r--r--   0        0        0      245 2023-06-08 18:28:14.905741 bruinen-1.1/src/bruinen/client/models/confirmation_status.py
+-rw-r--r--   0        0        0     1360 2023-06-08 18:28:16.014434 bruinen-1.1/src/bruinen/client/models/connection_requests_controller_find_all_response_200_item.py
+-rw-r--r--   0        0        0     3000 2023-06-08 18:28:16.032606 bruinen-1.1/src/bruinen/client/models/create_confirm_dto.py
+-rw-r--r--   0        0        0     1208 2023-06-08 18:28:16.010975 bruinen-1.1/src/bruinen/client/models/create_confirm_dto_params.py
+-rw-r--r--   0        0        0     2064 2023-06-08 18:28:16.028576 bruinen-1.1/src/bruinen/client/models/create_confirm_returned_dto.py
+-rw-r--r--   0        0        0     2988 2023-06-08 18:28:16.009520 bruinen-1.1/src/bruinen/client/models/create_connection_request_dto.py
+-rw-r--r--   0        0        0     1261 2023-06-08 18:28:16.001612 bruinen-1.1/src/bruinen/client/models/create_connection_request_dto_source.py
+-rw-r--r--   0        0        0     2362 2023-06-08 18:28:16.035990 bruinen-1.1/src/bruinen/client/models/create_user_dto.py
+-rw-r--r--   0        0        0      193 2023-06-08 18:28:14.841578 bruinen-1.1/src/bruinen/client/models/credential_provider.py
+-rw-r--r--   0        0        0     2141 2023-06-08 18:28:16.027659 bruinen-1.1/src/bruinen/client/models/endpoint_data.py
+-rw-r--r--   0        0        0     1165 2023-06-08 18:28:16.048060 bruinen-1.1/src/bruinen/client/models/get_response_200.py
+-rw-r--r--   0        0        0    13880 2023-06-08 18:28:16.184935 bruinen-1.1/src/bruinen/client/models/github_profile.py
+-rw-r--r--   0        0        0    27798 2023-06-08 18:28:16.300947 bruinen-1.1/src/bruinen/client/models/github_repo.py
+-rw-r--r--   0        0        0    13906 2023-06-08 18:28:16.187486 bruinen-1.1/src/bruinen/client/models/github_repo_owner.py
+-rw-r--r--   0        0        0     2751 2023-06-08 18:28:16.071648 bruinen-1.1/src/bruinen/client/models/github_repo_permissions.py
+-rw-r--r--   0        0        0     4464 2023-06-08 18:28:16.086672 bruinen-1.1/src/bruinen/client/models/google_calendar.py
+-rw-r--r--   0        0        0     2188 2023-06-08 18:28:16.051935 bruinen-1.1/src/bruinen/client/models/google_calendar_conference_properties.py
+-rw-r--r--   0        0        0     3595 2023-06-08 18:28:16.065820 bruinen-1.1/src/bruinen/client/models/google_calendars.py
+-rw-r--r--   0        0        0    10266 2023-06-08 18:28:16.139028 bruinen-1.1/src/bruinen/client/models/google_calendars_calendars_item.py
+-rw-r--r--   0        0        0     2264 2023-06-08 18:28:16.063952 bruinen-1.1/src/bruinen/client/models/google_calendars_calendars_item_conference_properties.py
+-rw-r--r--   0        0        0     2024 2023-06-08 18:28:16.079248 bruinen-1.1/src/bruinen/client/models/google_calendars_calendars_item_default_reminders.py
+-rw-r--r--   0        0        0     3002 2023-06-08 18:28:16.110138 bruinen-1.1/src/bruinen/client/models/google_calendars_calendars_item_notification_settings.py
+-rw-r--r--   0        0        0     2052 2023-06-08 18:28:16.109207 bruinen-1.1/src/bruinen/client/models/google_calendars_calendars_item_notification_settings_notifications_item.py
+-rw-r--r--   0        0        0     2268 2023-06-08 18:28:16.111688 bruinen-1.1/src/bruinen/client/models/google_draft.py
+-rw-r--r--   0        0        0     4723 2023-06-08 18:28:16.130243 bruinen-1.1/src/bruinen/client/models/google_draft_message.py
+-rw-r--r--   0        0        0     5102 2023-06-08 18:28:16.179941 bruinen-1.1/src/bruinen/client/models/google_draft_message_payload.py
+-rw-r--r--   0        0        0     2138 2023-06-08 18:28:16.148843 bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_body.py
+-rw-r--r--   0        0        0     1830 2023-06-08 18:28:16.131782 bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_headers_item.py
+-rw-r--r--   0        0        0     5385 2023-06-09 17:40:25.903009 bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_parts_item.py
+-rw-r--r--   0        0        0     2186 2023-06-08 18:28:16.156442 bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_parts_item_body.py
+-rw-r--r--   0        0        0     1881 2023-06-08 18:28:16.185959 bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_parts_item_headers_item.py
+-rw-r--r--   0        0        0     4547 2023-06-09 17:40:25.903159 bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item.py
+-rw-r--r--   0        0        0     1908 2023-06-09 17:40:25.903472 bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item_body.py
+-rw-r--r--   0        0        0     1932 2023-06-09 17:40:25.903944 bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item_headers_item.py
+-rw-r--r--   0        0        0     3038 2023-06-08 18:28:16.221038 bruinen-1.1/src/bruinen/client/models/google_drafts.py
+-rw-r--r--   0        0        0     2403 2023-06-08 18:28:16.217403 bruinen-1.1/src/bruinen/client/models/google_drafts_drafts_item.py
+-rw-r--r--   0        0        0     1887 2023-06-08 18:28:16.212333 bruinen-1.1/src/bruinen/client/models/google_drafts_drafts_item_message.py
+-rw-r--r--   0        0        0    21058 2023-06-08 18:28:16.382642 bruinen-1.1/src/bruinen/client/models/google_event.py
+-rw-r--r--   0        0        0     2812 2023-06-08 18:28:16.215955 bruinen-1.1/src/bruinen/client/models/google_event_attachments_item.py
+-rw-r--r--   0        0        0     4469 2023-06-08 18:28:16.236647 bruinen-1.1/src/bruinen/client/models/google_event_attendees_item.py
+-rw-r--r--   0        0        0     5871 2023-06-08 18:28:16.273066 bruinen-1.1/src/bruinen/client/models/google_event_conference_data.py
+-rw-r--r--   0        0        0     3028 2023-06-08 18:28:16.236836 bruinen-1.1/src/bruinen/client/models/google_event_conference_data_conference_solution.py
+-rw-r--r--   0        0        0     1694 2023-06-08 18:28:16.237269 bruinen-1.1/src/bruinen/client/models/google_event_conference_data_conference_solution_key.py
+-rw-r--r--   0        0        0     4265 2023-06-08 18:28:16.243956 bruinen-1.1/src/bruinen/client/models/google_event_conference_data_create_request.py
+-rw-r--r--   0        0        0     1796 2023-06-08 18:28:16.250244 bruinen-1.1/src/bruinen/client/models/google_event_conference_data_create_request_conference_solution_key.py
+-rw-r--r--   0        0        0     1766 2023-06-08 18:28:16.251524 bruinen-1.1/src/bruinen/client/models/google_event_conference_data_create_request_status.py
+-rw-r--r--   0        0        0     3860 2023-06-08 18:28:16.331458 bruinen-1.1/src/bruinen/client/models/google_event_conference_data_entry_points_item.py
+-rw-r--r--   0        0        0     2401 2023-06-08 18:28:16.271588 bruinen-1.1/src/bruinen/client/models/google_event_creator.py
+-rw-r--r--   0        0        0     2127 2023-06-08 18:28:16.259736 bruinen-1.1/src/bruinen/client/models/google_event_end.py
+-rw-r--r--   0        0        0     3226 2023-06-08 18:28:16.277257 bruinen-1.1/src/bruinen/client/models/google_event_extended_properties.py
+-rw-r--r--   0        0        0     1323 2023-06-08 18:28:16.264239 bruinen-1.1/src/bruinen/client/models/google_event_extended_properties_private.py
+-rw-r--r--   0        0        0     1317 2023-06-08 18:28:16.267989 bruinen-1.1/src/bruinen/client/models/google_event_extended_properties_shared.py
+-rw-r--r--   0        0        0     4170 2023-06-08 18:28:16.299896 bruinen-1.1/src/bruinen/client/models/google_event_gadget.py
+-rw-r--r--   0        0        0     1266 2023-06-08 18:28:16.285988 bruinen-1.1/src/bruinen/client/models/google_event_gadget_preferences.py
+-rw-r--r--   0        0        0     2421 2023-06-08 18:28:16.301608 bruinen-1.1/src/bruinen/client/models/google_event_organizer.py
+-rw-r--r--   0        0        0     2259 2023-06-08 18:28:16.300156 bruinen-1.1/src/bruinen/client/models/google_event_original_start_time.py
+-rw-r--r--   0        0        0     2753 2023-06-08 18:28:16.297782 bruinen-1.1/src/bruinen/client/models/google_event_reminders.py
+-rw-r--r--   0        0        0     1953 2023-06-08 18:28:16.313675 bruinen-1.1/src/bruinen/client/models/google_event_reminders_overrides_item.py
+-rw-r--r--   0        0        0     1785 2023-06-08 18:28:16.320407 bruinen-1.1/src/bruinen/client/models/google_event_source.py
+-rw-r--r--   0        0        0     2145 2023-06-08 18:28:16.322388 bruinen-1.1/src/bruinen/client/models/google_event_start.py
+-rw-r--r--   0        0        0     6772 2023-06-08 18:28:16.356798 bruinen-1.1/src/bruinen/client/models/google_events.py
+-rw-r--r--   0        0        0     1924 2023-06-08 18:28:16.315422 bruinen-1.1/src/bruinen/client/models/google_events_default_reminders_item.py
+-rw-r--r--   0        0        0    22193 2023-06-08 18:28:16.624572 bruinen-1.1/src/bruinen/client/models/google_events_events_item.py
+-rw-r--r--   0        0        0     2873 2023-06-08 18:28:16.340653 bruinen-1.1/src/bruinen/client/models/google_events_events_item_attachments_item.py
+-rw-r--r--   0        0        0     4530 2023-06-08 18:28:16.347976 bruinen-1.1/src/bruinen/client/models/google_events_events_item_attendees_item.py
+-rw-r--r--   0        0        0     6310 2023-06-08 18:28:16.365013 bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data.py
+-rw-r--r--   0        0        0     3181 2023-06-08 18:28:16.351105 bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution.py
+-rw-r--r--   0        0        0     1755 2023-06-08 18:28:16.448855 bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution_key.py
+-rw-r--r--   0        0        0     4541 2023-06-08 18:28:16.370930 bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request.py
+-rw-r--r--   0        0        0     1857 2023-06-08 18:28:16.359181 bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request_conference_solution_key.py
+-rw-r--r--   0        0        0     1827 2023-06-08 18:28:16.366254 bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request_status.py
+-rw-r--r--   0        0        0     3921 2023-06-08 18:28:16.419441 bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_entry_points_item.py
+-rw-r--r--   0        0        0     2462 2023-06-08 18:28:16.479859 bruinen-1.1/src/bruinen/client/models/google_events_events_item_creator.py
+-rw-r--r--   0        0        0     2188 2023-06-08 18:28:16.417085 bruinen-1.1/src/bruinen/client/models/google_events_events_item_end.py
+-rw-r--r--   0        0        0     3579 2023-06-08 18:28:16.452847 bruinen-1.1/src/bruinen/client/models/google_events_events_item_extended_properties.py
+-rw-r--r--   0        0        0     1384 2023-06-08 18:28:16.382966 bruinen-1.1/src/bruinen/client/models/google_events_events_item_extended_properties_private.py
+-rw-r--r--   0        0        0     1378 2023-06-08 18:28:16.407280 bruinen-1.1/src/bruinen/client/models/google_events_events_item_extended_properties_shared.py
+-rw-r--r--   0        0        0     4323 2023-06-08 18:28:16.457687 bruinen-1.1/src/bruinen/client/models/google_events_events_item_gadget.py
+-rw-r--r--   0        0        0     1327 2023-06-08 18:28:16.445942 bruinen-1.1/src/bruinen/client/models/google_events_events_item_gadget_preferences.py
+-rw-r--r--   0        0        0     2482 2023-06-08 18:28:16.447912 bruinen-1.1/src/bruinen/client/models/google_events_events_item_organizer.py
+-rw-r--r--   0        0        0     2320 2023-06-08 18:28:16.451846 bruinen-1.1/src/bruinen/client/models/google_events_events_item_original_start_time.py
+-rw-r--r--   0        0        0     2920 2023-06-08 18:28:16.469885 bruinen-1.1/src/bruinen/client/models/google_events_events_item_reminders.py
+-rw-r--r--   0        0        0     2014 2023-06-08 18:28:16.507659 bruinen-1.1/src/bruinen/client/models/google_events_events_item_reminders_overrides_item.py
+-rw-r--r--   0        0        0     1846 2023-06-08 18:28:16.484520 bruinen-1.1/src/bruinen/client/models/google_events_events_item_source.py
+-rw-r--r--   0        0        0     2206 2023-06-08 18:28:16.499456 bruinen-1.1/src/bruinen/client/models/google_events_events_item_start.py
+-rw-r--r--   0        0        0     5170 2023-06-08 18:28:16.516180 bruinen-1.1/src/bruinen/client/models/google_label.py
+-rw-r--r--   0        0        0     1927 2023-06-08 18:28:16.471978 bruinen-1.1/src/bruinen/client/models/google_label_color.py
+-rw-r--r--   0        0        0     2652 2023-06-08 18:28:16.503323 bruinen-1.1/src/bruinen/client/models/google_labels.py
+-rw-r--r--   0        0        0     2945 2023-06-08 18:28:16.497539 bruinen-1.1/src/bruinen/client/models/google_labels_labels_item.py
+-rw-r--r--   0        0        0     4411 2023-06-08 18:28:16.523945 bruinen-1.1/src/bruinen/client/models/google_message.py
+-rw-r--r--   0        0        0     4958 2023-06-08 18:28:16.525852 bruinen-1.1/src/bruinen/client/models/google_message_payload.py
+-rw-r--r--   0        0        0     2110 2023-06-08 18:28:16.511307 bruinen-1.1/src/bruinen/client/models/google_message_payload_body.py
+-rw-r--r--   0        0        0     1802 2023-06-08 18:28:16.521519 bruinen-1.1/src/bruinen/client/models/google_message_payload_headers_item.py
+-rw-r--r--   0        0        0     4162 2023-06-08 18:28:16.544691 bruinen-1.1/src/bruinen/client/models/google_message_payload_parts_item.py
+-rw-r--r--   0        0        0     2158 2023-06-08 18:28:16.531934 bruinen-1.1/src/bruinen/client/models/google_message_payload_parts_item_body.py
+-rw-r--r--   0        0        0     1853 2023-06-08 18:28:16.526662 bruinen-1.1/src/bruinen/client/models/google_message_payload_parts_item_headers_item.py
+-rw-r--r--   0        0        0     3115 2023-06-08 18:28:16.540904 bruinen-1.1/src/bruinen/client/models/google_messages.py
+-rw-r--r--   0        0        0     1844 2023-06-08 18:28:16.562328 bruinen-1.1/src/bruinen/client/models/google_messages_messages_item.py
+-rw-r--r--   0        0        0     4814 2023-06-09 17:40:25.904292 bruinen-1.1/src/bruinen/client/models/google_parsed_draft.py
+-rw-r--r--   0        0        0     3902 2023-06-09 17:40:25.904547 bruinen-1.1/src/bruinen/client/models/google_parsed_draft_attachments_item.py
+-rw-r--r--   0        0        0     5378 2023-06-09 17:40:25.904827 bruinen-1.1/src/bruinen/client/models/google_parsed_draft_headers.py
+-rw-r--r--   0        0        0     1865 2023-06-09 17:40:25.904963 bruinen-1.1/src/bruinen/client/models/google_parsed_draft_headers_bcc_item.py
+-rw-r--r--   0        0        0     1857 2023-06-09 17:40:25.905092 bruinen-1.1/src/bruinen/client/models/google_parsed_draft_headers_cc_item.py
+-rw-r--r--   0        0        0     1858 2023-06-09 17:40:25.905255 bruinen-1.1/src/bruinen/client/models/google_parsed_draft_headers_from.py
+-rw-r--r--   0        0        0     1879 2023-06-09 17:40:25.905494 bruinen-1.1/src/bruinen/client/models/google_parsed_draft_headers_to_item.py
+-rw-r--r--   0        0        0     4552 2023-06-09 17:40:25.905636 bruinen-1.1/src/bruinen/client/models/google_parsed_message.py
+-rw-r--r--   0        0        0     3914 2023-06-09 17:40:25.906023 bruinen-1.1/src/bruinen/client/models/google_parsed_message_attachments_item.py
+-rw-r--r--   0        0        0     5460 2023-06-09 17:40:25.906186 bruinen-1.1/src/bruinen/client/models/google_parsed_message_headers.py
+-rw-r--r--   0        0        0     1877 2023-06-09 17:40:25.906324 bruinen-1.1/src/bruinen/client/models/google_parsed_message_headers_bcc_item.py
+-rw-r--r--   0        0        0     1869 2023-06-09 17:40:25.906463 bruinen-1.1/src/bruinen/client/models/google_parsed_message_headers_cc_item.py
+-rw-r--r--   0        0        0     1870 2023-06-09 17:40:25.906712 bruinen-1.1/src/bruinen/client/models/google_parsed_message_headers_from.py
+-rw-r--r--   0        0        0     1891 2023-06-09 17:40:25.906856 bruinen-1.1/src/bruinen/client/models/google_parsed_message_headers_to_item.py
+-rw-r--r--   0        0        0     2583 2023-06-09 17:40:25.906993 bruinen-1.1/src/bruinen/client/models/google_parsed_thread.py
+-rw-r--r--   0        0        0     4837 2023-06-09 17:40:25.907194 bruinen-1.1/src/bruinen/client/models/google_parsed_thread_messages_item.py
+-rw-r--r--   0        0        0     3975 2023-06-09 17:40:25.907353 bruinen-1.1/src/bruinen/client/models/google_parsed_thread_messages_item_attachments_item.py
+-rw-r--r--   0        0        0     5948 2023-06-09 17:40:25.908088 bruinen-1.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers.py
+-rw-r--r--   0        0        0     1938 2023-06-09 17:40:25.908247 bruinen-1.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_bcc_item.py
+-rw-r--r--   0        0        0     1930 2023-06-09 17:40:25.908372 bruinen-1.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_cc_item.py
+-rw-r--r--   0        0        0     1931 2023-06-09 17:40:25.908487 bruinen-1.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_from.py
+-rw-r--r--   0        0        0     1952 2023-06-09 17:40:25.908616 bruinen-1.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_to_item.py
+-rw-r--r--   0        0        0     2662 2023-06-08 18:28:16.639671 bruinen-1.1/src/bruinen/client/models/google_profile.py
+-rw-r--r--   0        0        0     3121 2023-06-08 18:28:16.657045 bruinen-1.1/src/bruinen/client/models/google_thread.py
+-rw-r--r--   0        0        0     4544 2023-06-08 18:28:16.679730 bruinen-1.1/src/bruinen/client/models/google_thread_messages_item.py
+-rw-r--r--   0        0        0     5273 2023-06-08 18:28:16.675242 bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload.py
+-rw-r--r--   0        0        0     2171 2023-06-08 18:28:16.674238 bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload_body.py
+-rw-r--r--   0        0        0     1863 2023-06-08 18:28:16.653579 bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload_headers_item.py
+-rw-r--r--   0        0        0     4480 2023-06-08 18:28:16.674475 bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item.py
+-rw-r--r--   0        0        0     2219 2023-06-08 18:28:16.660948 bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_body.py
+-rw-r--r--   0        0        0     1914 2023-06-08 18:28:16.668112 bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_headers_item.py
+-rw-r--r--   0        0        0     3068 2023-06-08 18:28:16.687423 bruinen-1.1/src/bruinen/client/models/google_threads.py
+-rw-r--r--   0        0        0     2135 2023-06-08 18:28:16.692612 bruinen-1.1/src/bruinen/client/models/google_threads_threads_item.py
+-rw-r--r--   0        0        0     3499 2023-06-08 18:28:16.693297 bruinen-1.1/src/bruinen/client/models/returned_account_dto.py
+-rw-r--r--   0        0        0     4714 2023-06-08 18:28:16.716873 bruinen-1.1/src/bruinen/client/models/returned_confirm_dto.py
+-rw-r--r--   0        0        0     1218 2023-06-08 18:28:16.695101 bruinen-1.1/src/bruinen/client/models/returned_confirm_dto_params.py
+-rw-r--r--   0        0        0     3613 2023-06-08 18:28:16.702414 bruinen-1.1/src/bruinen/client/models/returned_connection_request_dto.py
+-rw-r--r--   0        0        0     1271 2023-06-08 18:28:16.688511 bruinen-1.1/src/bruinen/client/models/returned_connection_request_dto_source.py
+-rw-r--r--   0        0        0     4313 2023-06-08 18:28:16.716258 bruinen-1.1/src/bruinen/client/models/returned_source_policy_dto.py
+-rw-r--r--   0        0        0     2719 2023-06-08 18:28:16.718901 bruinen-1.1/src/bruinen/client/models/returned_user_dto.py
+-rw-r--r--   0        0        0     2901 2023-06-08 18:28:16.724385 bruinen-1.1/src/bruinen/client/models/source_data.py
+-rw-r--r--   0        0        0      177 2023-06-08 18:28:14.867040 bruinen-1.1/src/bruinen/client/models/source_policy_status.py
+-rw-r--r--   0        0        0      549 2023-06-08 18:28:14.819891 bruinen-1.1/src/bruinen/client/models/source_type.py
+-rw-r--r--   0        0        0     1350 2023-06-08 18:28:16.702821 bruinen-1.1/src/bruinen/client/models/sources_controller_get_metadata_for_source_response_200.py
+-rw-r--r--   0        0        0     2362 2023-06-08 18:28:16.714258 bruinen-1.1/src/bruinen/client/models/update_user_dto.py
+-rw-r--r--   0        0        0     2362 2023-06-08 18:28:16.715685 bruinen-1.1/src/bruinen/client/models/upsert_user_dto.py
+-rw-r--r--   0        0        0     1292 2023-06-08 18:28:16.713241 bruinen-1.1/src/bruinen/client/models/usage_controller_find_all_response_200_item.py
+-rw-r--r--   0        0        0       25 2023-06-08 18:28:13.955446 bruinen-1.1/src/bruinen/client/py.typed
+-rw-r--r--   0        0        0      993 2023-06-08 18:28:16.712632 bruinen-1.1/src/bruinen/client/types.py
+-rw-r--r--   0        0        0       36 2023-06-09 17:40:25.908847 bruinen-1.1/src/bruinen/confirm/__init__.py
+-rw-r--r--   0        0        0     2032 2023-05-30 21:25:54.185883 bruinen-1.1/src/bruinen/confirm/confirm.py
+-rw-r--r--   0        0        0        0 2023-05-30 21:25:54.185920 bruinen-1.1/src/bruinen/langchain/__init__.py
+-rw-r--r--   0        0        0     6484 2023-06-09 17:40:25.909335 bruinen-1.1/src/bruinen/langchain/github.py
+-rw-r--r--   0        0        0    52215 2023-06-09 17:40:25.909905 bruinen-1.1/src/bruinen/langchain/google.py
+-rw-r--r--   0        0        0       34 2023-06-06 18:24:40.536279 bruinen-1.1/src/bruinen/langchain/parsers/__init__.py
+-rw-r--r--   0        0        0     4398 2023-06-09 17:40:25.910512 bruinen-1.1/src/bruinen/langchain/parsers/sql_parser.py
+-rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 bruinen-1.1/PKG-INFO
```

### Comparing `bruinen-1.0/pyproject.toml` & `bruinen-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bruinen"
-version = "1.0"
+version = "1.1"
 description = "A client library for accessing Bruinen API"
 authors = []
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = ">=0.15.4,<0.25.0"
```

### Comparing `bruinen-1.0/src/bruinen/client/api/accounts/account_counts_for_policy.py` & `bruinen-1.1/src/bruinen/client/api/accounts/account_counts_for_policy.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/accounts/accounts_controller_deactivate.py` & `bruinen-1.1/src/bruinen/client/api/accounts/accounts_controller_deactivate.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/accounts/accounts_controller_get_accounts.py` & `bruinen-1.1/src/bruinen/client/api/accounts/accounts_controller_get_accounts.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/accounts/find_all_accounts_for_user.py` & `bruinen-1.1/src/bruinen/client/api/accounts/find_all_accounts_for_user.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/accounts/find_all_active_for_user.py` & `bruinen-1.1/src/bruinen/client/api/accounts/find_all_active_for_user.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/accounts/find_all_active_with_policy_for_user.py` & `bruinen-1.1/src/bruinen/client/api/accounts/find_all_active_with_policy_for_user.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/accounts/get_account.py` & `bruinen-1.1/src/bruinen/client/api/accounts/get_account.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/auth/get_user_auth_token.py` & `bruinen-1.1/src/bruinen/client/api/auth/get_user_auth_token.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/confirm/create.py` & `bruinen-1.1/src/bruinen/client/api/confirm/create.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/confirm/find_one.py` & `bruinen-1.1/src/bruinen/client/api/confirm/find_one.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/connection_requests/connection_requests_controller_find_all.py` & `bruinen-1.1/src/bruinen/client/api/connection_requests/connection_requests_controller_find_all.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/connection_requests/create.py` & `bruinen-1.1/src/bruinen/client/api/connection_requests/create.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/connection_requests/get.py` & `bruinen-1.1/src/bruinen/client/api/connection_requests/get.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/default/app_controller_get_hello.py` & `bruinen-1.1/src/bruinen/client/api/usage/usage_controller_get_client_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
+from ...models.client_usage_data import ClientUsageData
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/".format(client.base_url)
+    url = "{}/usage/client-data".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[str]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ClientUsageData]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = cast(str, response.json())
+        response_200 = ClientUsageData.from_dict(response.json())
+
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[str]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ClientUsageData]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[str]:
+) -> Response[ClientUsageData]:
     """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[str]
+        Response[ClientUsageData]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
@@ -70,40 +72,40 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[str]:
+) -> Optional[ClientUsageData]:
     """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        str
+        ClientUsageData
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[str]:
+) -> Response[ClientUsageData]:
     """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[str]
+        Response[ClientUsageData]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -111,22 +113,22 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[str]:
+) -> Optional[ClientUsageData]:
     """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        str
+        ClientUsageData
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `bruinen-1.0/src/bruinen/client/api/source_policy/source_policy_controller_deactivate.py` & `bruinen-1.1/src/bruinen/client/api/source_policy/source_policy_controller_set_default.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def _get_kwargs(
     id: Any,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/source-policy/deactivate/{id}".format(client.base_url, id=id)
+    url = "{}/source-policy/default/{id}".format(client.base_url, id=id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "patch",
         "url": url,
```

### Comparing `bruinen-1.0/src/bruinen/client/api/source_policy/source_policy_controller_get_all_active_for_client.py` & `bruinen-1.1/src/bruinen/client/api/source_policy/source_policy_controller_get_all_active_for_client.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/source_policy/source_policy_controller_get_defaults_for_client.py` & `bruinen-1.1/src/bruinen/client/api/source_policy/source_policy_controller_get_defaults_for_client.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/source_policy/source_policy_controller_get_policy_by_id.py` & `bruinen-1.1/src/bruinen/client/api/source_policy/source_policy_controller_get_policy_by_id.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/source_policy/source_policy_controller_set_default.py` & `bruinen-1.1/src/bruinen/client/api/sources/github_controller_repos.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,155 +1,166 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.returned_source_policy_dto import ReturnedSourcePolicyDto
-from ...types import Response
+from ...models.github_repo import GithubRepo
+from ...types import UNSET, Response
 
 
 def _get_kwargs(
-    id: Any,
     *,
     client: Client,
+    account_id: str,
 ) -> Dict[str, Any]:
-    url = "{}/source-policy/default/{id}".format(client.base_url, id=id)
+    url = "{}/sources/github/repos".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    params: Dict[str, Any] = {}
+    params["accountId"] = account_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
     return {
-        "method": "patch",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
+        "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ReturnedSourcePolicyDto]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List["GithubRepo"]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ReturnedSourcePolicyDto.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = GithubRepo.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ReturnedSourcePolicyDto]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[List["GithubRepo"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: Any,
     *,
     client: Client,
-) -> Response[ReturnedSourcePolicyDto]:
+    account_id: str,
+) -> Response[List["GithubRepo"]]:
     """
     Args:
-        id (Any):
+        account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ReturnedSourcePolicyDto]
+        Response[List['GithubRepo']]
     """
 
     kwargs = _get_kwargs(
-        id=id,
         client=client,
+        account_id=account_id,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    id: Any,
     *,
     client: Client,
-) -> Optional[ReturnedSourcePolicyDto]:
+    account_id: str,
+) -> Optional[List["GithubRepo"]]:
     """
     Args:
-        id (Any):
+        account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ReturnedSourcePolicyDto
+        List['GithubRepo']
     """
 
     return sync_detailed(
-        id=id,
         client=client,
+        account_id=account_id,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: Any,
     *,
     client: Client,
-) -> Response[ReturnedSourcePolicyDto]:
+    account_id: str,
+) -> Response[List["GithubRepo"]]:
     """
     Args:
-        id (Any):
+        account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ReturnedSourcePolicyDto]
+        Response[List['GithubRepo']]
     """
 
     kwargs = _get_kwargs(
-        id=id,
         client=client,
+        account_id=account_id,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    id: Any,
     *,
     client: Client,
-) -> Optional[ReturnedSourcePolicyDto]:
+    account_id: str,
+) -> Optional[List["GithubRepo"]]:
     """
     Args:
-        id (Any):
+        account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ReturnedSourcePolicyDto
+        List['GithubRepo']
     """
 
     return (
         await asyncio_detailed(
-            id=id,
             client=client,
+            account_id=account_id,
         )
     ).parsed
```

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/github_controller_get_auth_callback.py` & `bruinen-1.1/src/bruinen/client/api/sources/sources_controller_get_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/sources/github/callback".format(client.base_url)
+    url = "{}/sources/metadata".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
```

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/github_controller_profile.py` & `bruinen-1.1/src/bruinen/client/api/sources/github_controller_profile.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/github_controller_repos.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_draft.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.github_repo import GithubRepo
+from ...models.google_draft import GoogleDraft
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
     client: Client,
+    draft_id: str,
     account_id: str,
 ) -> Dict[str, Any]:
-    url = "{}/sources/github/repos".format(client.base_url)
+    url = "{}/sources/google/draft".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
+    params["draftId"] = draft_id
+
     params["accountId"] = account_id
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
@@ -31,136 +34,143 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List["GithubRepo"]]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GoogleDraft]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = GithubRepo.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
+        response_200 = GoogleDraft.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[List["GithubRepo"]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GoogleDraft]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
+    draft_id: str,
     account_id: str,
-) -> Response[List["GithubRepo"]]:
+) -> Response[GoogleDraft]:
     """
     Args:
+        draft_id (str):
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['GithubRepo']]
+        Response[GoogleDraft]
     """
 
     kwargs = _get_kwargs(
         client=client,
+        draft_id=draft_id,
         account_id=account_id,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
+    draft_id: str,
     account_id: str,
-) -> Optional[List["GithubRepo"]]:
+) -> Optional[GoogleDraft]:
     """
     Args:
+        draft_id (str):
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['GithubRepo']
+        GoogleDraft
     """
 
     return sync_detailed(
         client=client,
+        draft_id=draft_id,
         account_id=account_id,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
+    draft_id: str,
     account_id: str,
-) -> Response[List["GithubRepo"]]:
+) -> Response[GoogleDraft]:
     """
     Args:
+        draft_id (str):
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['GithubRepo']]
+        Response[GoogleDraft]
     """
 
     kwargs = _get_kwargs(
         client=client,
+        draft_id=draft_id,
         account_id=account_id,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
+    draft_id: str,
     account_id: str,
-) -> Optional[List["GithubRepo"]]:
+) -> Optional[GoogleDraft]:
     """
     Args:
+        draft_id (str):
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['GithubRepo']
+        GoogleDraft
     """
 
     return (
         await asyncio_detailed(
             client=client,
+            draft_id=draft_id,
             account_id=account_id,
         )
     ).parsed
```

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_calendar.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_calendar.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_calendars.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_calendars.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_draft.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_parsed_draft.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.google_draft import GoogleDraft
+from ...models.google_parsed_draft import GoogleParsedDraft
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
     client: Client,
     draft_id: str,
     account_id: str,
 ) -> Dict[str, Any]:
-    url = "{}/sources/google/draft".format(client.base_url)
+    url = "{}/sources/google/parsedDraft".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["draftId"] = draft_id
 
@@ -34,51 +34,51 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GoogleDraft]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GoogleParsedDraft]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GoogleDraft.from_dict(response.json())
+        response_200 = GoogleParsedDraft.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GoogleDraft]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GoogleParsedDraft]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
     draft_id: str,
     account_id: str,
-) -> Response[GoogleDraft]:
+) -> Response[GoogleParsedDraft]:
     """
     Args:
         draft_id (str):
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GoogleDraft]
+        Response[GoogleParsedDraft]
     """
 
     kwargs = _get_kwargs(
         client=client,
         draft_id=draft_id,
         account_id=account_id,
     )
@@ -92,52 +92,52 @@
 
 
 def sync(
     *,
     client: Client,
     draft_id: str,
     account_id: str,
-) -> Optional[GoogleDraft]:
+) -> Optional[GoogleParsedDraft]:
     """
     Args:
         draft_id (str):
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GoogleDraft
+        GoogleParsedDraft
     """
 
     return sync_detailed(
         client=client,
         draft_id=draft_id,
         account_id=account_id,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
     draft_id: str,
     account_id: str,
-) -> Response[GoogleDraft]:
+) -> Response[GoogleParsedDraft]:
     """
     Args:
         draft_id (str):
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GoogleDraft]
+        Response[GoogleParsedDraft]
     """
 
     kwargs = _get_kwargs(
         client=client,
         draft_id=draft_id,
         account_id=account_id,
     )
@@ -149,26 +149,26 @@
 
 
 async def asyncio(
     *,
     client: Client,
     draft_id: str,
     account_id: str,
-) -> Optional[GoogleDraft]:
+) -> Optional[GoogleParsedDraft]:
     """
     Args:
         draft_id (str):
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GoogleDraft
+        GoogleParsedDraft
     """
 
     return (
         await asyncio_detailed(
             client=client,
             draft_id=draft_id,
             account_id=account_id,
```

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_drafts.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_drafts.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_event.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_event.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_events.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_events.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_get_auth_callback.py` & `bruinen-1.1/src/bruinen/client/api/usage/usage_controller_find_one.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 
 from ... import errors
 from ...client import Client
 from ...types import Response
 
 
 def _get_kwargs(
+    id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/sources/google/callback".format(client.base_url)
+    url = "{}/usage/byId/{id}".format(client.base_url, id=id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
@@ -42,52 +43,62 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    id: str,
     *,
     client: Client,
 ) -> Response[Any]:
     """
+    Args:
+        id (str):
+
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
+    id: str,
     *,
     client: Client,
 ) -> Response[Any]:
     """
+    Args:
+        id (str):
+
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
```

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_label.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_label.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_labels.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_labels.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_message.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_message.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_messages.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_messages.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_profile.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_profile.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_thread.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_thread.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/google_controller_threads.py` & `bruinen-1.1/src/bruinen/client/api/sources/google_controller_threads.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/sources/sources_controller_get_metadata_for_source.py` & `bruinen-1.1/src/bruinen/client/api/sources/sources_controller_get_metadata_for_source.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/usage/usage_controller_find_all.py` & `bruinen-1.1/src/bruinen/client/api/usage/usage_controller_find_all.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/usage/usage_controller_find_one.py` & `bruinen-1.1/src/bruinen/client/api/users/users_controller_find_all.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,104 +1,139 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
+from ...models.returned_user_dto import ReturnedUserDto
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/usage/byId/{id}".format(client.base_url, id=id)
+    url = "{}/users/all".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List["ReturnedUserDto"]]:
     if response.status_code == HTTPStatus.OK:
-        return None
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = ReturnedUserDto.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
+
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[List["ReturnedUserDto"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: str,
     *,
     client: Client,
-) -> Response[Any]:
+) -> Response[List["ReturnedUserDto"]]:
     """
-    Args:
-        id (str):
-
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[List['ReturnedUserDto']]
     """
 
     kwargs = _get_kwargs(
-        id=id,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio_detailed(
-    id: str,
+def sync(
     *,
     client: Client,
-) -> Response[Any]:
+) -> Optional[List["ReturnedUserDto"]]:
     """
-    Args:
-        id (str):
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
+    Returns:
+        List['ReturnedUserDto']
+    """
+
+    return sync_detailed(
+        client=client,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: Client,
+) -> Response[List["ReturnedUserDto"]]:
+    """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[List['ReturnedUserDto']]
     """
 
     kwargs = _get_kwargs(
-        id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: Client,
+) -> Optional[List["ReturnedUserDto"]]:
+    """
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        List['ReturnedUserDto']
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `bruinen-1.0/src/bruinen/client/api/users/users_controller_create.py` & `bruinen-1.1/src/bruinen/client/api/users/users_controller_create.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/users/users_controller_find_all.py` & `bruinen-1.1/src/bruinen/client/api/users/users_controller_find_one.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,139 +1,155 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
 from ...models.returned_user_dto import ReturnedUserDto
 from ...types import Response
 
 
 def _get_kwargs(
+    id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/users/all".format(client.base_url)
+    url = "{}/users/byId/{id}".format(client.base_url, id=id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List["ReturnedUserDto"]]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ReturnedUserDto]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = ReturnedUserDto.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
+        response_200 = ReturnedUserDto.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[List["ReturnedUserDto"]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ReturnedUserDto]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    id: str,
     *,
     client: Client,
-) -> Response[List["ReturnedUserDto"]]:
+) -> Response[ReturnedUserDto]:
     """
+    Args:
+        id (str):
+
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ReturnedUserDto']]
+        Response[ReturnedUserDto]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    id: str,
     *,
     client: Client,
-) -> Optional[List["ReturnedUserDto"]]:
+) -> Optional[ReturnedUserDto]:
     """
+    Args:
+        id (str):
+
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['ReturnedUserDto']
+        ReturnedUserDto
     """
 
     return sync_detailed(
+        id=id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    id: str,
     *,
     client: Client,
-) -> Response[List["ReturnedUserDto"]]:
+) -> Response[ReturnedUserDto]:
     """
+    Args:
+        id (str):
+
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ReturnedUserDto']]
+        Response[ReturnedUserDto]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    id: str,
     *,
     client: Client,
-) -> Optional[List["ReturnedUserDto"]]:
+) -> Optional[ReturnedUserDto]:
     """
+    Args:
+        id (str):
+
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['ReturnedUserDto']
+        ReturnedUserDto
     """
 
     return (
         await asyncio_detailed(
+            id=id,
             client=client,
         )
     ).parsed
```

### Comparing `bruinen-1.0/src/bruinen/client/api/users/users_controller_find_one.py` & `bruinen-1.1/src/bruinen/client/api/users/users_controller_upsert_user.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,42 +2,46 @@
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
 from ...models.returned_user_dto import ReturnedUserDto
+from ...models.upsert_user_dto import UpsertUserDto
 from ...types import Response
 
 
 def _get_kwargs(
-    id: str,
     *,
     client: Client,
+    json_body: UpsertUserDto,
 ) -> Dict[str, Any]:
-    url = "{}/users/byId/{id}".format(client.base_url, id=id)
+    url = "{}/users/upsert".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "get",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ReturnedUserDto]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = ReturnedUserDto.from_dict(response.json())
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = ReturnedUserDto.from_dict(response.json())
 
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[ReturnedUserDto]:
@@ -46,110 +50,110 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    id: str,
     *,
     client: Client,
+    json_body: UpsertUserDto,
 ) -> Response[ReturnedUserDto]:
     """
     Args:
-        id (str):
+        json_body (UpsertUserDto):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ReturnedUserDto]
     """
 
     kwargs = _get_kwargs(
-        id=id,
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    id: str,
     *,
     client: Client,
+    json_body: UpsertUserDto,
 ) -> Optional[ReturnedUserDto]:
     """
     Args:
-        id (str):
+        json_body (UpsertUserDto):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         ReturnedUserDto
     """
 
     return sync_detailed(
-        id=id,
         client=client,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
-    id: str,
     *,
     client: Client,
+    json_body: UpsertUserDto,
 ) -> Response[ReturnedUserDto]:
     """
     Args:
-        id (str):
+        json_body (UpsertUserDto):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ReturnedUserDto]
     """
 
     kwargs = _get_kwargs(
-        id=id,
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    id: str,
     *,
     client: Client,
+    json_body: UpsertUserDto,
 ) -> Optional[ReturnedUserDto]:
     """
     Args:
-        id (str):
+        json_body (UpsertUserDto):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         ReturnedUserDto
     """
 
     return (
         await asyncio_detailed(
-            id=id,
             client=client,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `bruinen-1.0/src/bruinen/client/api/users/users_controller_find_user_from_token.py` & `bruinen-1.1/src/bruinen/client/api/users/users_controller_find_user_from_token.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/api/users/users_controller_update.py` & `bruinen-1.1/src/bruinen/client/api/users/users_controller_update.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/client.py` & `bruinen-1.1/src/bruinen/client/client.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/__init__.py` & `bruinen-1.1/src/bruinen/client/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 from .google_draft_message import GoogleDraftMessage
 from .google_draft_message_payload import GoogleDraftMessagePayload
 from .google_draft_message_payload_body import GoogleDraftMessagePayloadBody
 from .google_draft_message_payload_headers_item import GoogleDraftMessagePayloadHeadersItem
 from .google_draft_message_payload_parts_item import GoogleDraftMessagePayloadPartsItem
 from .google_draft_message_payload_parts_item_body import GoogleDraftMessagePayloadPartsItemBody
 from .google_draft_message_payload_parts_item_headers_item import GoogleDraftMessagePayloadPartsItemHeadersItem
+from .google_draft_message_payload_parts_item_parts_item import GoogleDraftMessagePayloadPartsItemPartsItem
+from .google_draft_message_payload_parts_item_parts_item_body import GoogleDraftMessagePayloadPartsItemPartsItemBody
+from .google_draft_message_payload_parts_item_parts_item_headers_item import (
+    GoogleDraftMessagePayloadPartsItemPartsItemHeadersItem,
+)
 from .google_drafts import GoogleDrafts
 from .google_drafts_drafts_item import GoogleDraftsDraftsItem
 from .google_drafts_drafts_item_message import GoogleDraftsDraftsItemMessage
 from .google_event import GoogleEvent
 from .google_event_attachments_item import GoogleEventAttachmentsItem
 from .google_event_attendees_item import GoogleEventAttendeesItem
 from .google_event_conference_data import GoogleEventConferenceData
@@ -112,14 +117,36 @@
 from .google_message_payload_body import GoogleMessagePayloadBody
 from .google_message_payload_headers_item import GoogleMessagePayloadHeadersItem
 from .google_message_payload_parts_item import GoogleMessagePayloadPartsItem
 from .google_message_payload_parts_item_body import GoogleMessagePayloadPartsItemBody
 from .google_message_payload_parts_item_headers_item import GoogleMessagePayloadPartsItemHeadersItem
 from .google_messages import GoogleMessages
 from .google_messages_messages_item import GoogleMessagesMessagesItem
+from .google_parsed_draft import GoogleParsedDraft
+from .google_parsed_draft_attachments_item import GoogleParsedDraftAttachmentsItem
+from .google_parsed_draft_headers import GoogleParsedDraftHeaders
+from .google_parsed_draft_headers_bcc_item import GoogleParsedDraftHeadersBccItem
+from .google_parsed_draft_headers_cc_item import GoogleParsedDraftHeadersCcItem
+from .google_parsed_draft_headers_from import GoogleParsedDraftHeadersFrom
+from .google_parsed_draft_headers_to_item import GoogleParsedDraftHeadersToItem
+from .google_parsed_message import GoogleParsedMessage
+from .google_parsed_message_attachments_item import GoogleParsedMessageAttachmentsItem
+from .google_parsed_message_headers import GoogleParsedMessageHeaders
+from .google_parsed_message_headers_bcc_item import GoogleParsedMessageHeadersBccItem
+from .google_parsed_message_headers_cc_item import GoogleParsedMessageHeadersCcItem
+from .google_parsed_message_headers_from import GoogleParsedMessageHeadersFrom
+from .google_parsed_message_headers_to_item import GoogleParsedMessageHeadersToItem
+from .google_parsed_thread import GoogleParsedThread
+from .google_parsed_thread_messages_item import GoogleParsedThreadMessagesItem
+from .google_parsed_thread_messages_item_attachments_item import GoogleParsedThreadMessagesItemAttachmentsItem
+from .google_parsed_thread_messages_item_headers import GoogleParsedThreadMessagesItemHeaders
+from .google_parsed_thread_messages_item_headers_bcc_item import GoogleParsedThreadMessagesItemHeadersBccItem
+from .google_parsed_thread_messages_item_headers_cc_item import GoogleParsedThreadMessagesItemHeadersCcItem
+from .google_parsed_thread_messages_item_headers_from import GoogleParsedThreadMessagesItemHeadersFrom
+from .google_parsed_thread_messages_item_headers_to_item import GoogleParsedThreadMessagesItemHeadersToItem
 from .google_profile import GoogleProfile
 from .google_thread import GoogleThread
 from .google_thread_messages_item import GoogleThreadMessagesItem
 from .google_thread_messages_item_payload import GoogleThreadMessagesItemPayload
 from .google_thread_messages_item_payload_body import GoogleThreadMessagesItemPayloadBody
 from .google_thread_messages_item_payload_headers_item import GoogleThreadMessagesItemPayloadHeadersItem
 from .google_thread_messages_item_payload_parts_item import GoogleThreadMessagesItemPayloadPartsItem
@@ -177,14 +204,17 @@
     "GoogleDraftMessage",
     "GoogleDraftMessagePayload",
     "GoogleDraftMessagePayloadBody",
     "GoogleDraftMessagePayloadHeadersItem",
     "GoogleDraftMessagePayloadPartsItem",
     "GoogleDraftMessagePayloadPartsItemBody",
     "GoogleDraftMessagePayloadPartsItemHeadersItem",
+    "GoogleDraftMessagePayloadPartsItemPartsItem",
+    "GoogleDraftMessagePayloadPartsItemPartsItemBody",
+    "GoogleDraftMessagePayloadPartsItemPartsItemHeadersItem",
     "GoogleDrafts",
     "GoogleDraftsDraftsItem",
     "GoogleDraftsDraftsItemMessage",
     "GoogleEvent",
     "GoogleEventAttachmentsItem",
     "GoogleEventAttendeesItem",
     "GoogleEventConferenceData",
@@ -241,14 +271,36 @@
     "GoogleMessagePayloadBody",
     "GoogleMessagePayloadHeadersItem",
     "GoogleMessagePayloadPartsItem",
     "GoogleMessagePayloadPartsItemBody",
     "GoogleMessagePayloadPartsItemHeadersItem",
     "GoogleMessages",
     "GoogleMessagesMessagesItem",
+    "GoogleParsedDraft",
+    "GoogleParsedDraftAttachmentsItem",
+    "GoogleParsedDraftHeaders",
+    "GoogleParsedDraftHeadersBccItem",
+    "GoogleParsedDraftHeadersCcItem",
+    "GoogleParsedDraftHeadersFrom",
+    "GoogleParsedDraftHeadersToItem",
+    "GoogleParsedMessage",
+    "GoogleParsedMessageAttachmentsItem",
+    "GoogleParsedMessageHeaders",
+    "GoogleParsedMessageHeadersBccItem",
+    "GoogleParsedMessageHeadersCcItem",
+    "GoogleParsedMessageHeadersFrom",
+    "GoogleParsedMessageHeadersToItem",
+    "GoogleParsedThread",
+    "GoogleParsedThreadMessagesItem",
+    "GoogleParsedThreadMessagesItemAttachmentsItem",
+    "GoogleParsedThreadMessagesItemHeaders",
+    "GoogleParsedThreadMessagesItemHeadersBccItem",
+    "GoogleParsedThreadMessagesItemHeadersCcItem",
+    "GoogleParsedThreadMessagesItemHeadersFrom",
+    "GoogleParsedThreadMessagesItemHeadersToItem",
     "GoogleProfile",
     "GoogleThread",
     "GoogleThreadMessagesItem",
     "GoogleThreadMessagesItemPayload",
     "GoogleThreadMessagesItemPayloadBody",
     "GoogleThreadMessagesItemPayloadHeadersItem",
     "GoogleThreadMessagesItemPayloadPartsItem",
```

### Comparing `bruinen-1.0/src/bruinen/client/models/accounts_controller_deactivate_response_200.py` & `bruinen-1.1/src/bruinen/client/models/accounts_controller_deactivate_response_200.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/accounts_controller_get_accounts_response_200_item.py` & `bruinen-1.1/src/bruinen/client/models/accounts_controller_get_accounts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/auth.py` & `bruinen-1.1/src/bruinen/client/models/auth.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/client_usage_data.py` & `bruinen-1.1/src/bruinen/client/models/client_usage_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/connection_requests_controller_find_all_response_200_item.py` & `bruinen-1.1/src/bruinen/client/models/connection_requests_controller_find_all_response_200_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/create_confirm_dto.py` & `bruinen-1.1/src/bruinen/client/models/create_confirm_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/create_confirm_dto_params.py` & `bruinen-1.1/src/bruinen/client/models/create_confirm_dto_params.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/create_confirm_returned_dto.py` & `bruinen-1.1/src/bruinen/client/models/create_confirm_returned_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/create_connection_request_dto.py` & `bruinen-1.1/src/bruinen/client/models/create_connection_request_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/create_connection_request_dto_source.py` & `bruinen-1.1/src/bruinen/client/models/create_connection_request_dto_source.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/create_user_dto.py` & `bruinen-1.1/src/bruinen/client/models/create_user_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/endpoint_data.py` & `bruinen-1.1/src/bruinen/client/models/endpoint_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/get_response_200.py` & `bruinen-1.1/src/bruinen/client/models/get_response_200.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/github_profile.py` & `bruinen-1.1/src/bruinen/client/models/github_profile.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/github_repo.py` & `bruinen-1.1/src/bruinen/client/models/github_repo.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/github_repo_owner.py` & `bruinen-1.1/src/bruinen/client/models/github_repo_owner.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/github_repo_permissions.py` & `bruinen-1.1/src/bruinen/client/models/github_repo_permissions.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_calendar.py` & `bruinen-1.1/src/bruinen/client/models/google_calendar.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_calendar_conference_properties.py` & `bruinen-1.1/src/bruinen/client/models/google_calendar_conference_properties.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_calendars.py` & `bruinen-1.1/src/bruinen/client/models/google_calendars.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_calendars_calendars_item.py` & `bruinen-1.1/src/bruinen/client/models/google_calendars_calendars_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_calendars_calendars_item_conference_properties.py` & `bruinen-1.1/src/bruinen/client/models/google_calendars_calendars_item_conference_properties.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_calendars_calendars_item_default_reminders.py` & `bruinen-1.1/src/bruinen/client/models/google_calendars_calendars_item_default_reminders.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_calendars_calendars_item_notification_settings.py` & `bruinen-1.1/src/bruinen/client/models/google_calendars_calendars_item_notification_settings.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_calendars_calendars_item_notification_settings_notifications_item.py` & `bruinen-1.1/src/bruinen/client/models/google_calendars_calendars_item_notification_settings_notifications_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_draft.py` & `bruinen-1.1/src/bruinen/client/models/google_draft.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_draft_message.py` & `bruinen-1.1/src/bruinen/client/models/google_draft_message.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_draft_message_payload.py` & `bruinen-1.1/src/bruinen/client/models/google_draft_message_payload.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_draft_message_payload_body.py` & `bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_draft_message_payload_headers_item.py` & `bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_draft_message_payload_parts_item.py` & `bruinen-1.1/src/bruinen/client/models/google_message_payload_parts_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.google_draft_message_payload_parts_item_body import GoogleDraftMessagePayloadPartsItemBody
-    from ..models.google_draft_message_payload_parts_item_headers_item import (
-        GoogleDraftMessagePayloadPartsItemHeadersItem,
-    )
+    from ..models.google_message_payload_parts_item_body import GoogleMessagePayloadPartsItemBody
+    from ..models.google_message_payload_parts_item_headers_item import GoogleMessagePayloadPartsItemHeadersItem
 
 
-T = TypeVar("T", bound="GoogleDraftMessagePayloadPartsItem")
+T = TypeVar("T", bound="GoogleMessagePayloadPartsItem")
 
 
 @attr.s(auto_attribs=True)
-class GoogleDraftMessagePayloadPartsItem:
+class GoogleMessagePayloadPartsItem:
     """
     Attributes:
         part_id (Union[Unset, str]): The partId of the part
         mime_type (Union[Unset, str]): The mimeType of the part
         filename (Union[Unset, str]): The filename of the part
-        headers (Union[Unset, List['GoogleDraftMessagePayloadPartsItemHeadersItem']]): The headers of the part
-        body (Union[Unset, GoogleDraftMessagePayloadPartsItemBody]): The body of the part
+        headers (Union[Unset, List['GoogleMessagePayloadPartsItemHeadersItem']]): The headers of the part
+        body (Union[Unset, GoogleMessagePayloadPartsItemBody]): The body of the part
     """
 
     part_id: Union[Unset, str] = UNSET
     mime_type: Union[Unset, str] = UNSET
     filename: Union[Unset, str] = UNSET
-    headers: Union[Unset, List["GoogleDraftMessagePayloadPartsItemHeadersItem"]] = UNSET
-    body: Union[Unset, "GoogleDraftMessagePayloadPartsItemBody"] = UNSET
+    headers: Union[Unset, List["GoogleMessagePayloadPartsItemHeadersItem"]] = UNSET
+    body: Union[Unset, "GoogleMessagePayloadPartsItemBody"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         part_id = self.part_id
         mime_type = self.mime_type
         filename = self.filename
         headers: Union[Unset, List[Dict[str, Any]]] = UNSET
@@ -62,50 +60,48 @@
         if body is not UNSET:
             field_dict["body"] = body
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.google_draft_message_payload_parts_item_body import GoogleDraftMessagePayloadPartsItemBody
-        from ..models.google_draft_message_payload_parts_item_headers_item import (
-            GoogleDraftMessagePayloadPartsItemHeadersItem,
-        )
+        from ..models.google_message_payload_parts_item_body import GoogleMessagePayloadPartsItemBody
+        from ..models.google_message_payload_parts_item_headers_item import GoogleMessagePayloadPartsItemHeadersItem
 
         d = src_dict.copy()
         part_id = d.pop("partId", UNSET) or UNSET
 
         mime_type = d.pop("mimeType", UNSET) or UNSET
 
         filename = d.pop("filename", UNSET) or UNSET
 
         headers = []
         _headers = d.pop("headers", UNSET) or UNSET
         for headers_item_data in _headers or []:
-            headers_item = GoogleDraftMessagePayloadPartsItemHeadersItem.from_dict(headers_item_data)
+            headers_item = GoogleMessagePayloadPartsItemHeadersItem.from_dict(headers_item_data)
 
             headers.append(headers_item)
 
         _body = d.pop("body", UNSET) or UNSET
-        body: Union[Unset, GoogleDraftMessagePayloadPartsItemBody]
+        body: Union[Unset, GoogleMessagePayloadPartsItemBody]
         if isinstance(_body, Unset):
             body = UNSET
         else:
-            body = GoogleDraftMessagePayloadPartsItemBody.from_dict(_body)
+            body = GoogleMessagePayloadPartsItemBody.from_dict(_body)
 
-        google_draft_message_payload_parts_item = cls(
+        google_message_payload_parts_item = cls(
             part_id=part_id,
             mime_type=mime_type,
             filename=filename,
             headers=headers,
             body=body,
         )
 
-        google_draft_message_payload_parts_item.additional_properties = d
-        return google_draft_message_payload_parts_item
+        google_message_payload_parts_item.additional_properties = d
+        return google_message_payload_parts_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `bruinen-1.0/src/bruinen/client/models/google_draft_message_payload_parts_item_body.py` & `bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_parts_item_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_draft_message_payload_parts_item_headers_item.py` & `bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_parts_item_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_drafts.py` & `bruinen-1.1/src/bruinen/client/models/google_drafts.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_drafts_drafts_item.py` & `bruinen-1.1/src/bruinen/client/models/google_drafts_drafts_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_drafts_drafts_item_message.py` & `bruinen-1.1/src/bruinen/client/models/google_drafts_drafts_item_message.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event.py` & `bruinen-1.1/src/bruinen/client/models/google_event.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_attachments_item.py` & `bruinen-1.1/src/bruinen/client/models/google_event_attachments_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_attendees_item.py` & `bruinen-1.1/src/bruinen/client/models/google_event_attendees_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_conference_data.py` & `bruinen-1.1/src/bruinen/client/models/google_event_conference_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_conference_data_conference_solution.py` & `bruinen-1.1/src/bruinen/client/models/google_event_conference_data_conference_solution.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_conference_data_conference_solution_key.py` & `bruinen-1.1/src/bruinen/client/models/google_event_conference_data_conference_solution_key.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_conference_data_create_request.py` & `bruinen-1.1/src/bruinen/client/models/google_event_conference_data_create_request.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_conference_data_create_request_conference_solution_key.py` & `bruinen-1.1/src/bruinen/client/models/google_event_conference_data_create_request_conference_solution_key.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_conference_data_create_request_status.py` & `bruinen-1.1/src/bruinen/client/models/google_event_conference_data_create_request_status.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_conference_data_entry_points_item.py` & `bruinen-1.1/src/bruinen/client/models/google_event_conference_data_entry_points_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_creator.py` & `bruinen-1.1/src/bruinen/client/models/google_event_creator.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_end.py` & `bruinen-1.1/src/bruinen/client/models/google_event_end.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_extended_properties.py` & `bruinen-1.1/src/bruinen/client/models/google_event_extended_properties.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_extended_properties_private.py` & `bruinen-1.1/src/bruinen/client/models/google_event_extended_properties_private.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_extended_properties_shared.py` & `bruinen-1.1/src/bruinen/client/models/google_event_extended_properties_shared.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_gadget.py` & `bruinen-1.1/src/bruinen/client/models/google_event_gadget.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_gadget_preferences.py` & `bruinen-1.1/src/bruinen/client/models/google_event_gadget_preferences.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_organizer.py` & `bruinen-1.1/src/bruinen/client/models/google_event_organizer.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_original_start_time.py` & `bruinen-1.1/src/bruinen/client/models/google_event_original_start_time.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_reminders.py` & `bruinen-1.1/src/bruinen/client/models/google_event_reminders.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_reminders_overrides_item.py` & `bruinen-1.1/src/bruinen/client/models/google_event_reminders_overrides_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_source.py` & `bruinen-1.1/src/bruinen/client/models/google_event_source.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_event_start.py` & `bruinen-1.1/src/bruinen/client/models/google_event_start.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events.py` & `bruinen-1.1/src/bruinen/client/models/google_events.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_default_reminders_item.py` & `bruinen-1.1/src/bruinen/client/models/google_events_default_reminders_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_attachments_item.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_attachments_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_attendees_item.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_attendees_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution_key.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution_key.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_create_request.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_create_request_conference_solution_key.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request_conference_solution_key.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_create_request_status.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request_status.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_conference_data_entry_points_item.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_conference_data_entry_points_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_creator.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_creator.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_end.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_end.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_extended_properties.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_extended_properties.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_extended_properties_private.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_extended_properties_private.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_extended_properties_shared.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_extended_properties_shared.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_gadget.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_gadget.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_gadget_preferences.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_gadget_preferences.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_organizer.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_organizer.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_original_start_time.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_original_start_time.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_reminders.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_reminders.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_reminders_overrides_item.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_reminders_overrides_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_source.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_source.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_events_events_item_start.py` & `bruinen-1.1/src/bruinen/client/models/google_events_events_item_start.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_label.py` & `bruinen-1.1/src/bruinen/client/models/google_label.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_label_color.py` & `bruinen-1.1/src/bruinen/client/models/google_label_color.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_labels.py` & `bruinen-1.1/src/bruinen/client/models/google_labels.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_labels_labels_item.py` & `bruinen-1.1/src/bruinen/client/models/google_labels_labels_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_message.py` & `bruinen-1.1/src/bruinen/client/models/google_message.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_message_payload.py` & `bruinen-1.1/src/bruinen/client/models/google_message_payload.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_message_payload_body.py` & `bruinen-1.1/src/bruinen/client/models/google_message_payload_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_message_payload_headers_item.py` & `bruinen-1.1/src/bruinen/client/models/google_message_payload_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_message_payload_parts_item.py` & `bruinen-1.1/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.google_message_payload_parts_item_body import GoogleMessagePayloadPartsItemBody
-    from ..models.google_message_payload_parts_item_headers_item import GoogleMessagePayloadPartsItemHeadersItem
+    from ..models.google_draft_message_payload_parts_item_parts_item_body import (
+        GoogleDraftMessagePayloadPartsItemPartsItemBody,
+    )
+    from ..models.google_draft_message_payload_parts_item_parts_item_headers_item import (
+        GoogleDraftMessagePayloadPartsItemPartsItemHeadersItem,
+    )
 
 
-T = TypeVar("T", bound="GoogleMessagePayloadPartsItem")
+T = TypeVar("T", bound="GoogleDraftMessagePayloadPartsItemPartsItem")
 
 
 @attr.s(auto_attribs=True)
-class GoogleMessagePayloadPartsItem:
+class GoogleDraftMessagePayloadPartsItemPartsItem:
     """
     Attributes:
         part_id (Union[Unset, str]): The partId of the part
         mime_type (Union[Unset, str]): The mimeType of the part
         filename (Union[Unset, str]): The filename of the part
-        headers (Union[Unset, List['GoogleMessagePayloadPartsItemHeadersItem']]): The headers of the part
-        body (Union[Unset, GoogleMessagePayloadPartsItemBody]): The body of the part
+        headers (Union[Unset, List['GoogleDraftMessagePayloadPartsItemPartsItemHeadersItem']]): The headers of the part
+        body (Union[Unset, GoogleDraftMessagePayloadPartsItemPartsItemBody]): The body of the part
     """
 
     part_id: Union[Unset, str] = UNSET
     mime_type: Union[Unset, str] = UNSET
     filename: Union[Unset, str] = UNSET
-    headers: Union[Unset, List["GoogleMessagePayloadPartsItemHeadersItem"]] = UNSET
-    body: Union[Unset, "GoogleMessagePayloadPartsItemBody"] = UNSET
+    headers: Union[Unset, List["GoogleDraftMessagePayloadPartsItemPartsItemHeadersItem"]] = UNSET
+    body: Union[Unset, "GoogleDraftMessagePayloadPartsItemPartsItemBody"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         part_id = self.part_id
         mime_type = self.mime_type
         filename = self.filename
         headers: Union[Unset, List[Dict[str, Any]]] = UNSET
@@ -60,48 +64,52 @@
         if body is not UNSET:
             field_dict["body"] = body
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.google_message_payload_parts_item_body import GoogleMessagePayloadPartsItemBody
-        from ..models.google_message_payload_parts_item_headers_item import GoogleMessagePayloadPartsItemHeadersItem
+        from ..models.google_draft_message_payload_parts_item_parts_item_body import (
+            GoogleDraftMessagePayloadPartsItemPartsItemBody,
+        )
+        from ..models.google_draft_message_payload_parts_item_parts_item_headers_item import (
+            GoogleDraftMessagePayloadPartsItemPartsItemHeadersItem,
+        )
 
         d = src_dict.copy()
         part_id = d.pop("partId", UNSET) or UNSET
 
         mime_type = d.pop("mimeType", UNSET) or UNSET
 
         filename = d.pop("filename", UNSET) or UNSET
 
         headers = []
         _headers = d.pop("headers", UNSET) or UNSET
         for headers_item_data in _headers or []:
-            headers_item = GoogleMessagePayloadPartsItemHeadersItem.from_dict(headers_item_data)
+            headers_item = GoogleDraftMessagePayloadPartsItemPartsItemHeadersItem.from_dict(headers_item_data)
 
             headers.append(headers_item)
 
         _body = d.pop("body", UNSET) or UNSET
-        body: Union[Unset, GoogleMessagePayloadPartsItemBody]
+        body: Union[Unset, GoogleDraftMessagePayloadPartsItemPartsItemBody]
         if isinstance(_body, Unset):
             body = UNSET
         else:
-            body = GoogleMessagePayloadPartsItemBody.from_dict(_body)
+            body = GoogleDraftMessagePayloadPartsItemPartsItemBody.from_dict(_body)
 
-        google_message_payload_parts_item = cls(
+        google_draft_message_payload_parts_item_parts_item = cls(
             part_id=part_id,
             mime_type=mime_type,
             filename=filename,
             headers=headers,
             body=body,
         )
 
-        google_message_payload_parts_item.additional_properties = d
-        return google_message_payload_parts_item
+        google_draft_message_payload_parts_item_parts_item.additional_properties = d
+        return google_draft_message_payload_parts_item_parts_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `bruinen-1.0/src/bruinen/client/models/google_message_payload_parts_item_body.py` & `bruinen-1.1/src/bruinen/client/models/google_message_payload_parts_item_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_message_payload_parts_item_headers_item.py` & `bruinen-1.1/src/bruinen/client/models/google_message_payload_parts_item_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_messages.py` & `bruinen-1.1/src/bruinen/client/models/google_messages.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_messages_messages_item.py` & `bruinen-1.1/src/bruinen/client/models/google_messages_messages_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_profile.py` & `bruinen-1.1/src/bruinen/client/models/google_profile.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_thread.py` & `bruinen-1.1/src/bruinen/client/models/google_thread.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_thread_messages_item.py` & `bruinen-1.1/src/bruinen/client/models/google_thread_messages_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload.py` & `bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload_body.py` & `bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload_headers_item.py` & `bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload_parts_item.py` & `bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_body.py` & `bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_headers_item.py` & `bruinen-1.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_threads.py` & `bruinen-1.1/src/bruinen/client/models/google_threads.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/google_threads_threads_item.py` & `bruinen-1.1/src/bruinen/client/models/google_threads_threads_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/returned_account_dto.py` & `bruinen-1.1/src/bruinen/client/models/returned_account_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/returned_confirm_dto.py` & `bruinen-1.1/src/bruinen/client/models/returned_confirm_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/returned_confirm_dto_params.py` & `bruinen-1.1/src/bruinen/client/models/returned_confirm_dto_params.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/returned_connection_request_dto.py` & `bruinen-1.1/src/bruinen/client/models/returned_connection_request_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/returned_connection_request_dto_source.py` & `bruinen-1.1/src/bruinen/client/models/returned_connection_request_dto_source.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/returned_source_policy_dto.py` & `bruinen-1.1/src/bruinen/client/models/returned_source_policy_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/returned_user_dto.py` & `bruinen-1.1/src/bruinen/client/models/returned_user_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/source_data.py` & `bruinen-1.1/src/bruinen/client/models/source_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/source_type.py` & `bruinen-1.1/src/bruinen/client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/sources_controller_get_metadata_for_source_response_200.py` & `bruinen-1.1/src/bruinen/client/models/sources_controller_get_metadata_for_source_response_200.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/update_user_dto.py` & `bruinen-1.1/src/bruinen/client/models/update_user_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/upsert_user_dto.py` & `bruinen-1.1/src/bruinen/client/models/upsert_user_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/models/usage_controller_find_all_response_200_item.py` & `bruinen-1.1/src/bruinen/client/models/usage_controller_find_all_response_200_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/client/types.py` & `bruinen-1.1/src/bruinen/client/types.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/confirm/confirm.py` & `bruinen-1.1/src/bruinen/confirm/confirm.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.0/src/bruinen/langchain/github.py` & `bruinen-1.1/src/bruinen/langchain/github.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from langchain.base_language import BaseLanguageModel
 from langchain.callbacks.manager import AsyncCallbackManagerForToolRun, CallbackManagerForToolRun
 from langchain.output_parsers import PydanticOutputParser
 from langchain.prompts.prompt import PromptTemplate
 from langchain.tools import BaseTool
 from pydantic import BaseModel, Field
 from typing import Callable, List, Optional
+from urllib.parse import quote
 
 from ..client import AuthenticatedClient
 from ..client.api.accounts import find_all_accounts_for_user
 from ..client.api.auth import get_user_auth_token
 from ..client.models import Auth, ReturnedAccountDto
 from ..client.types import Response
 
@@ -24,31 +25,39 @@
 class GithubAuthenticatorTool(BaseTool):
     name = 'Github Authenticator Tool'
     description = """Useful for when a user's Github account is not authenticated.
 
     Input to the tool should be an empty string.
 
     The response from the tool will be a URL that you return to the user for them to complete auth.
+    The URL will be your final answer.
     """
-    # Could add: This URL will be your final answer.
 
     client: AuthenticatedClient
-    server: str
     user_id: str
+    server: str = 'https://ui.bruinen.co'
+    source_policy_id: str = None
+    redirect_url: str
 
     def _run(
         self,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None
     ) -> str:
         """Run the tool."""
         response: Response[Auth] = get_user_auth_token.sync_detailed(client=self.client, user_id=self.user_id)
-        auth_token = response.parsed.access_token
-        # TODO decide how this URL should be formatted
-        return self.server + '?userToken=' + auth_token + '&source=google'
+        user_token = response.parsed.access_token
+
+        if self.source_policy_id is not None:
+            source = [{ 'name': 'github', 'sourcePolicyId': self.source_policy_id }]
+        else:
+            source = [{ 'name': 'github' }]
+        encoded_source = quote(json.dumps(source))
+        
+        return self.server + '/connect' + '?userToken=' + quote(user_token) + '&sources=' + encoded_source + '&defaultRedirectUrl=' + quote(self.redirect_url)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
```

### Comparing `bruinen-1.0/src/bruinen/langchain/google.py` & `bruinen-1.1/src/bruinen/langchain/google.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,39 +4,46 @@
 from langchain.base_language import BaseLanguageModel
 from langchain.callbacks.manager import AsyncCallbackManagerForToolRun, CallbackManagerForToolRun
 from langchain.output_parsers import PydanticOutputParser
 from langchain.prompts.prompt import PromptTemplate
 from langchain.tools import BaseTool
 from pydantic import BaseModel, Field
 from typing import Callable, List, Optional
+from urllib.parse import quote
 
 from ..client import AuthenticatedClient
 from ..client.api.accounts import find_all_accounts_for_user
 from ..client.api.auth import get_user_auth_token
 from ..client.models import Auth, ReturnedAccountDto
 from ..client.types import Response
 
 from ..client.api.sources import google_controller_profile
 from ..client.models import GoogleProfile
 from ..client.api.sources import google_controller_drafts
 from ..client.models import GoogleDrafts
 from ..client.api.sources import google_controller_draft
 from ..client.models import GoogleDraft
+from ..client.api.sources import google_controller_parsed_draft
+from ..client.models import GoogleParsedDraft
 from ..client.api.sources import google_controller_labels
 from ..client.models import GoogleLabels
 from ..client.api.sources import google_controller_label
 from ..client.models import GoogleLabel
 from ..client.api.sources import google_controller_messages
 from ..client.models import GoogleMessages
 from ..client.api.sources import google_controller_message
 from ..client.models import GoogleMessage
+from ..client.api.sources import google_controller_parsed_message
+from ..client.models import GoogleParsedMessage
 from ..client.api.sources import google_controller_threads
 from ..client.models import GoogleThreads
 from ..client.api.sources import google_controller_thread
 from ..client.models import GoogleThread
+from ..client.api.sources import google_controller_parsed_thread
+from ..client.models import GoogleParsedThread
 from ..client.api.sources import google_controller_calendars
 from ..client.models import GoogleCalendars
 from ..client.api.sources import google_controller_calendar
 from ..client.models import GoogleCalendar
 from ..client.api.sources import google_controller_events
 from ..client.models import GoogleEvents
 from ..client.api.sources import google_controller_event
@@ -46,31 +53,39 @@
 class GoogleAuthenticatorTool(BaseTool):
     name = 'Google Authenticator Tool'
     description = """Useful for when a user's Google account is not authenticated.
 
     Input to the tool should be an empty string.
 
     The response from the tool will be a URL that you return to the user for them to complete auth.
+    The URL will be your final answer.
     """
-    # Could add: This URL will be your final answer.
 
     client: AuthenticatedClient
-    server: str
     user_id: str
+    server: str = 'https://ui.bruinen.co'
+    source_policy_id: str = None
+    redirect_url: str
 
     def _run(
         self,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None
     ) -> str:
         """Run the tool."""
         response: Response[Auth] = get_user_auth_token.sync_detailed(client=self.client, user_id=self.user_id)
-        auth_token = response.parsed.access_token
-        # TODO decide how this URL should be formatted
-        return self.server + '?userToken=' + auth_token + '&source=google'
+        user_token = response.parsed.access_token
+
+        if self.source_policy_id is not None:
+            source = [{ 'name': 'google', 'sourcePolicyId': self.source_policy_id }]
+        else:
+            source = [{ 'name': 'google' }]
+        encoded_source = quote(json.dumps(source))
+        
+        return self.server + '/connect' + '?userToken=' + quote(user_token) + '&sources=' + encoded_source + '&defaultRedirectUrl=' + quote(self.redirect_url)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
@@ -130,27 +145,17 @@
         return await self._run(query, run_manager)
 
 
 class GoogleGetDraftsTool(BaseTool):
     name = "Google Get Drafts Tool"
     description = """Useful for when you need to get a user's Google drafts.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
-
-    The first line should be the question that you want to know the answer to.
-
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
-    
-    "q" (Optional), string: "The query for your drafts"
-    "pageToken" (Optional), string: "The page token for your drafts"
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleDrafts], str]] = None
@@ -158,29 +163,28 @@
     def _run(self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None) -> str:
         """Run the tool."""
 
         class GoogleGetDraftsToolInputSchema(BaseModel):
             q: Optional[str] = Field(description="The query for your drafts")
             pageToken: Optional[str] = Field(description="The page token for your drafts")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetDraftsToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -202,15 +206,15 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google drafts."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
@@ -218,55 +222,45 @@
         return await self._run(query, run_manager)
 
 
 class GoogleGetDraftTool(BaseTool):
     name = "Google Get Draft Tool"
     description = """Useful for when you need to get a user's Google draft.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
-
-    The first line should be the question that you want to know the answer to.
-
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
-    
-    "draftId" (Required), string: "The id of the draft"
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleDraft], str]] = None
 
     def _run(self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None) -> str:
         """Run the tool."""
 
         class GoogleGetDraftToolInputSchema(BaseModel):
             draftId: str = Field(description="The id of the draft")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetDraftToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -287,15 +281,90 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google draft."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
+
+    # TODO implement async version
+    async def _arun(
+        self,
+        query: str,
+        run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
+    ) -> str:
+        """Run the tool asynchronously."""
+        return await self._run(query, run_manager)
+
+
+class GoogleGetParsedDraftTool(BaseTool):
+    name = "Google Get ParsedDraft Tool"
+    description = """Useful for when you need to get a user's Google parsed_draft.
+    
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
+    
+    Output will be the text response from the Google API.
+    """
+
+    client: AuthenticatedClient
+    llm: BaseLanguageModel
+    user_id: str
+    parse_output: Optional[Callable[[GoogleParsedDraft], str]] = None
+
+    def _run(self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None) -> str:
+        """Run the tool."""
+
+        class GoogleGetParsedDraftToolInputSchema(BaseModel):
+            draftId: str = Field(description="The id of the draft")
+            
+        
+        parser = PydanticOutputParser(pydantic_object=GoogleGetParsedDraftToolInputSchema)
+        
+        prompt = PromptTemplate(
+            template="""Parse the provided input string.
+            For values that are not marked as required, if no value is provided, return a null value.
+            {format_instructions}
+            Here is the input:
+            {query}""",
+            input_variables=["query"],
+            partial_variables={"format_instructions": parser.get_format_instructions()},
+        )
+
+        _input = prompt.format_prompt(query=query)
+        output = self.llm(_input.to_string())
+        parsed_parameters = parser.parse(output)
+        
+        response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
+            client=self.client, user_id=self.user_id
+        )
+        if not 200 <= response.status_code < 300:
+            return "Error pulling the user's Google account."
+        accounts: List["ReturnedAccountDto"] = response.parsed
+
+        account_id = ""
+        for account in accounts:
+            if account.source == "google":
+                account_id = account.id
+        if account_id == "":
+            return "The user has not connected their Google account; you should try authenticating Google first."
+        else:
+            response: Response[GoogleParsedDraft] = google_controller_parsed_draft.sync_detailed(
+                client=self.client,
+                account_id=account_id,
+                draft_id=parsed_parameters.draftId
+            )
+            if not 200 <= response.status_code < 300:
+                return "Error when attempting to get the user's Google parsed_draft."
+
+            if self.parse_output is None:
+                return json.dumps(response.parsed.to_dict())
+            else:
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
@@ -355,55 +424,45 @@
         return await self._run(query, run_manager)
 
 
 class GoogleGetLabelTool(BaseTool):
     name = "Google Get Label Tool"
     description = """Useful for when you need to get a user's Google label.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
-
-    The first line should be the question that you want to know the answer to.
-
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    "labelId" (Required), string: "The id of the label"
-    
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleLabel], str]] = None
 
     def _run(self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None) -> str:
         """Run the tool."""
 
         class GoogleGetLabelToolInputSchema(BaseModel):
             labelId: str = Field(description="The id of the label")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetLabelToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -424,15 +483,15 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google label."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
@@ -440,28 +499,17 @@
         return await self._run(query, run_manager)
 
 
 class GoogleGetMessagesTool(BaseTool):
     name = "Google Get Messages Tool"
     description = """Useful for when you need to get a user's Google messages.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
-
-    The first line should be the question that you want to know the answer to.
-
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    "q" (Optional), string: "The query of the messages"
-    "pageToken" (Optional), string: "The pageToken of the messages"
-    "labelIds" (Optional), string: "The labelIds of the messages"
-    
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleMessages], str]] = None
@@ -470,29 +518,28 @@
         """Run the tool."""
 
         class GoogleGetMessagesToolInputSchema(BaseModel):
             q: Optional[str] = Field(description="The query of the messages")
             pageToken: Optional[str] = Field(description="The pageToken of the messages")
             labelIds: Optional[str] = Field(description="The labelIds of the messages")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetMessagesToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -515,15 +562,15 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google messages."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
@@ -531,55 +578,45 @@
         return await self._run(query, run_manager)
 
 
 class GoogleGetMessageTool(BaseTool):
     name = "Google Get Message Tool"
     description = """Useful for when you need to get a user's Google message.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
-
-    The first line should be the question that you want to know the answer to.
-
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    "messageId" (Required), string: "The id of the message"
-    
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleMessage], str]] = None
 
     def _run(self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None) -> str:
         """Run the tool."""
 
         class GoogleGetMessageToolInputSchema(BaseModel):
             messageId: str = Field(description="The id of the message")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetMessageToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -600,44 +637,108 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google message."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
-class GoogleGetThreadsTool(BaseTool):
-    name = "Google Get Threads Tool"
-    description = """Useful for when you need to get a user's Google threads.
+class GoogleGetParsedMessageTool(BaseTool):
+    name = "Google Get ParsedMessage Tool"
+    description = """Useful for when you need to get a user's Google parsed_message.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
+    
+    Output will be the text response from the Google API.
+    """
+
+    client: AuthenticatedClient
+    llm: BaseLanguageModel
+    user_id: str
+    parse_output: Optional[Callable[[GoogleParsedMessage], str]] = None
+
+    def _run(self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None) -> str:
+        """Run the tool."""
+
+        class GoogleGetParsedMessageToolInputSchema(BaseModel):
+            messageId: str = Field(description="The id of the message")
+            
+        
+        parser = PydanticOutputParser(pydantic_object=GoogleGetParsedMessageToolInputSchema)
+        
+        prompt = PromptTemplate(
+            template="""Parse the provided input string.
+            For values that are not marked as required, if no value is provided, return a null value.
+            {format_instructions}
+            Here is the input:
+            {query}""",
+            input_variables=["query"],
+            partial_variables={"format_instructions": parser.get_format_instructions()},
+        )
+
+        _input = prompt.format_prompt(query=query)
+        output = self.llm(_input.to_string())
+        parsed_parameters = parser.parse(output)
+        
+        response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
+            client=self.client, user_id=self.user_id
+        )
+        if not 200 <= response.status_code < 300:
+            return "Error pulling the user's Google account."
+        accounts: List["ReturnedAccountDto"] = response.parsed
+
+        account_id = ""
+        for account in accounts:
+            if account.source == "google":
+                account_id = account.id
+        if account_id == "":
+            return "The user has not connected their Google account; you should try authenticating Google first."
+        else:
+            response: Response[GoogleParsedMessage] = google_controller_parsed_message.sync_detailed(
+                client=self.client,
+                account_id=account_id,
+                message_id=parsed_parameters.messageId
+            )
+            if not 200 <= response.status_code < 300:
+                return "Error when attempting to get the user's Google parsed_message."
+
+            if self.parse_output is None:
+                return json.dumps(response.parsed.to_dict())
+            else:
+                return self.parse_output(response.parsed, query)
+
+    # TODO implement async version
+    async def _arun(
+        self,
+        query: str,
+        run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
+    ) -> str:
+        """Run the tool asynchronously."""
+        return await self._run(query, run_manager)
 
-    The first line should be the question that you want to know the answer to.
 
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
+class GoogleGetThreadsTool(BaseTool):
+    name = "Google Get Threads Tool"
+    description = """Useful for when you need to get a user's Google threads.
     
-    "q" (Optional), string: "The query of the threads"
-    "pageToken" (Optional), string: "The pageToken of the threads"
-    "labelIds" (Optional), string: "The labelIds of the threads"
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleThreads], str]] = None
@@ -646,29 +747,28 @@
         """Run the tool."""
 
         class GoogleGetThreadsToolInputSchema(BaseModel):
             q: Optional[str] = Field(description="The query of the threads")
             pageToken: Optional[str] = Field(description="The pageToken of the threads")
             labelIds: Optional[str] = Field(description="The labelIds of the threads")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetThreadsToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -691,15 +791,15 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google threads."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
@@ -707,55 +807,45 @@
         return await self._run(query, run_manager)
 
 
 class GoogleGetThreadTool(BaseTool):
     name = "Google Get Thread Tool"
     description = """Useful for when you need to get a user's Google thread.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
-
-    The first line should be the question that you want to know the answer to.
-
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    "threadId" (Required), string: "The id of the thread"
-    
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleThread], str]] = None
 
     def _run(self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None) -> str:
         """Run the tool."""
 
         class GoogleGetThreadToolInputSchema(BaseModel):
             threadId: str = Field(description="The id of the thread")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetThreadToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -776,45 +866,108 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google thread."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
-class GoogleGetCalendarsTool(BaseTool):
-    name = "Google Get Calendars Tool"
-    description = """Useful for when you need to get a user's Google calendars.
+class GoogleGetParsedThreadTool(BaseTool):
+    name = "Google Get ParsedThread Tool"
+    description = """Useful for when you need to get a user's Google parsed_thread.
+    
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
+    Output will be the text response from the Google API.
+    """
+
+    client: AuthenticatedClient
+    llm: BaseLanguageModel
+    user_id: str
+    parse_output: Optional[Callable[[GoogleParsedThread], str]] = None
 
-    The first line should be the question that you want to know the answer to.
+    def _run(self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None) -> str:
+        """Run the tool."""
 
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
+        class GoogleGetParsedThreadToolInputSchema(BaseModel):
+            threadId: str = Field(description="The id of the thread")
+            
+        
+        parser = PydanticOutputParser(pydantic_object=GoogleGetParsedThreadToolInputSchema)
+        
+        prompt = PromptTemplate(
+            template="""Parse the provided input string.
+            For values that are not marked as required, if no value is provided, return a null value.
+            {format_instructions}
+            Here is the input:
+            {query}""",
+            input_variables=["query"],
+            partial_variables={"format_instructions": parser.get_format_instructions()},
+        )
+
+        _input = prompt.format_prompt(query=query)
+        output = self.llm(_input.to_string())
+        parsed_parameters = parser.parse(output)
+        
+        response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
+            client=self.client, user_id=self.user_id
+        )
+        if not 200 <= response.status_code < 300:
+            return "Error pulling the user's Google account."
+        accounts: List["ReturnedAccountDto"] = response.parsed
+
+        account_id = ""
+        for account in accounts:
+            if account.source == "google":
+                account_id = account.id
+        if account_id == "":
+            return "The user has not connected their Google account; you should try authenticating Google first."
+        else:
+            response: Response[GoogleParsedThread] = google_controller_parsed_thread.sync_detailed(
+                client=self.client,
+                account_id=account_id,
+                thread_id=parsed_parameters.threadId
+            )
+            if not 200 <= response.status_code < 300:
+                return "Error when attempting to get the user's Google parsed_thread."
+
+            if self.parse_output is None:
+                return json.dumps(response.parsed.to_dict())
+            else:
+                return self.parse_output(response.parsed, query)
+
+    # TODO implement async version
+    async def _arun(
+        self,
+        query: str,
+        run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
+    ) -> str:
+        """Run the tool asynchronously."""
+        return await self._run(query, run_manager)
+
+
+class GoogleGetCalendarsTool(BaseTool):
+    name = "Google Get Calendars Tool"
+    description = """Useful for when you need to get a user's Google calendars.
     
-    "syncToken" (Optional), string: "The syncToken of the calendars"
-    "showHidden" (Optional), boolean: "Whether to show hidden calendars"
-    "showDeleted" (Optional), boolean: "Whether to show deleted calendars"
-    "pageToken" (Optional), string: "The pageToken of the calendars"
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleCalendars], str]] = None
@@ -824,29 +977,28 @@
 
         class GoogleGetCalendarsToolInputSchema(BaseModel):
             syncToken: Optional[str] = Field(description="The syncToken of the calendars")
             showHidden: Optional[bool] = Field(description="Whether to show hidden calendars")
             showDeleted: Optional[bool] = Field(description="Whether to show deleted calendars")
             pageToken: Optional[str] = Field(description="The pageToken of the calendars")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetCalendarsToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -870,15 +1022,15 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google calendars."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
@@ -886,55 +1038,45 @@
         return await self._run(query, run_manager)
 
 
 class GoogleGetCalendarTool(BaseTool):
     name = "Google Get Calendar Tool"
     description = """Useful for when you need to get a user's Google calendar.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
-
-    The first line should be the question that you want to know the answer to.
-
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
-    
-    "calendarId" (Required), string: "The id of the calendar"
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleCalendar], str]] = None
 
     def _run(self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None) -> str:
         """Run the tool."""
 
         class GoogleGetCalendarToolInputSchema(BaseModel):
             calendarId: str = Field(description="The id of the calendar")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetCalendarToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -955,15 +1097,15 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google calendar."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
@@ -971,38 +1113,17 @@
         return await self._run(query, run_manager)
 
 
 class GoogleGetEventsTool(BaseTool):
     name = "Google Get Events Tool"
     description = """Useful for when you need to get a user's Google events.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
-
-    The first line should be the question that you want to know the answer to.
-
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
-    
-    "iCalUID" (Optional), string: "The iCal UID"
-    "syncToken" (Optional), string: "The sync token"
-    "updatedMin" (Optional), string: "The updated min"
-    "timeZone" (Optional), string: "The time zone"
-    "timeMin" (Optional), string: "The time min"
-    "timeMax" (Optional), string: "The time max"
-    "singleEvents" (Optional), boolean: "Whether to show single events"
-    "showDeleted" (Optional), boolean: "Whether to show deleted"
-    "q" (Optional), string: "The query"
-    "pageToken" (Optional), string: "The page token"
-    "orderBy" (Optional), string: "The order by"
-    "maxAttendees" (Optional), number: "The max attendees"
-    "calendarId" (Optional), string: "The id of the calendar"
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleEvents], str]] = None
@@ -1021,29 +1142,28 @@
             showDeleted: Optional[bool] = Field(description="Whether to show deleted")
             q: Optional[str] = Field(description="The query")
             pageToken: Optional[str] = Field(description="The page token")
             orderBy: Optional[str] = Field(description="The order by")
             maxAttendees: Optional[int] = Field(description="The max attendees")
             calendarId: Optional[str] = Field(description="The id of the calendar")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetEventsToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -1076,15 +1196,15 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google events."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
@@ -1092,28 +1212,17 @@
         return await self._run(query, run_manager)
 
 
 class GoogleGetEventTool(BaseTool):
     name = "Google Get Event Tool"
     description = """Useful for when you need to get a user's Google event.
     
-    The input should be a string with two parts, separated by a new line character '\n'.
-    Always include the '\n' in the input, even if the second line is empty.
-
-    The first line should be the question that you want to know the answer to.
-
-    The second line should be the requested parameters to the Google API, as key/value pairs, separated by commas. 
-    For keys that are not marked as required, if no value is provided, do not include the key.
-    Possible keys for the the second line are:
-    
-    "timeZone" (Optional), string: "The timeZone of the event"
-    "eventId" (Required), string: "The id of the event"
-    "calendarId" (Required), string: "The calendarId of the calendar which contains the event"
+    Input should be a string containing the question that you want to know the answer to.
+    Do not pass parameters as JSON, instead pass the string to the tool as is.
     
-    If no parameters are provided, pass "No parameters" as the second line.
     Output will be the text response from the Google API.
     """
 
     client: AuthenticatedClient
     llm: BaseLanguageModel
     user_id: str
     parse_output: Optional[Callable[[GoogleEvent], str]] = None
@@ -1122,29 +1231,28 @@
         """Run the tool."""
 
         class GoogleGetEventToolInputSchema(BaseModel):
             timeZone: Optional[str] = Field(description="The timeZone of the event")
             eventId: str = Field(description="The id of the event")
             calendarId: str = Field(description="The calendarId of the calendar which contains the event")
             
-        question, raw_parameters = query.split("\n", 1)
         
         parser = PydanticOutputParser(pydantic_object=GoogleGetEventToolInputSchema)
         
         prompt = PromptTemplate(
             template="""Parse the provided input string.
             For values that are not marked as required, if no value is provided, return a null value.
             {format_instructions}
             Here is the input:
             {query}""",
             input_variables=["query"],
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
 
-        _input = prompt.format_prompt(query=raw_parameters)
+        _input = prompt.format_prompt(query=query)
         output = self.llm(_input.to_string())
         parsed_parameters = parser.parse(output)
         
         response: Response[List["ReturnedAccountDto"]] = find_all_accounts_for_user.sync_detailed(
             client=self.client, user_id=self.user_id
         )
         if not 200 <= response.status_code < 300:
@@ -1167,15 +1275,15 @@
             )
             if not 200 <= response.status_code < 300:
                 return "Error when attempting to get the user's Google event."
 
             if self.parse_output is None:
                 return json.dumps(response.parsed.to_dict())
             else:
-                return self.parse_output(response.parsed, question)
+                return self.parse_output(response.parsed, query)
 
     # TODO implement async version
     async def _arun(
         self,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
```

### Comparing `bruinen-1.0/src/bruinen/langchain/parsers/sql_parser.py` & `bruinen-1.1/src/bruinen/langchain/parsers/sql_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,29 @@
 from datetime import datetime
 from typing import ForwardRef, Union, get_args, get_origin
 
 from langchain import SQLDatabase, SQLDatabaseChain
 from langchain.base_language import BaseLanguageModel
 from langchain.prompts.prompt import PromptTemplate
-from sqlalchemy import (
-    JSON,
-    Boolean,
-    Column,
-    DateTime,
-    Float,
-    Integer,
-    MetaData,
-    String,
-    Table,
-    create_engine,
-)
+from sqlalchemy import JSON, Boolean, Column, DateTime, Float, Integer, MetaData, String, Table, create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.schema import CreateTable
 
 from ...client.types import Unset
 
 
 class SQLParser:
     def __init__(self, llm: BaseLanguageModel):
         self.llm = llm
 
     def parse(self, input, query):
         # Check if the input is a list (the SQL parser is only available for resources that return lists)
         if not (isinstance(input, list) or get_origin(input) is list):
-            raise TypeError(
-                "SQL parser is only available for resources that return lists"
-            )
+            raise TypeError("SQL parser is only available for resources that return lists")
 
         input_class = type(input[0])
         input_class_name = input_class.__name__
 
         class_attrs = {
             "__tablename__": input_class_name.lower(),
             "temporary_id": Column(Integer, primary_key=True),
@@ -59,29 +46,23 @@
             elif get_origin(type_var) is dict:
                 return JSON
             elif get_origin(type_var) is list:
                 return JSON
             elif type(type_var) == ForwardRef:
                 return JSON
             else:
-                raise ValueError(
-                    f"Unknown type when mapping Typing to SQLAlchemy: {type_var}"
-                )
+                raise ValueError(f"Unknown type when mapping Typing to SQLAlchemy: {type_var}")
 
         # TODO check if there's a better way to pull these
         for field_name, field_type in input_class.__dict__["__annotations__"].items():
             if get_origin(field_type) is Union:
                 # First argument should be Unset, otherwise raise an error
                 if get_args(field_type)[0] is not Unset:
-                    raise ValueError(
-                        "Union type with first value not Unset not supported"
-                    )
-                class_attrs[field_name] = Column(
-                    map_sql_types(get_args(field_type)[1]), nullable=True
-                )
+                    raise ValueError("Union type with first value not Unset not supported")
+                class_attrs[field_name] = Column(map_sql_types(get_args(field_type)[1]), nullable=True)
             else:
                 class_attrs[field_name] = Column(map_sql_types(field_type))
 
         engine = create_engine(f"sqlite:///{input_class_name.lower()}.db", echo=True)
         Base = declarative_base()
         sql_class = type(input_class_name, (Base,), class_attrs)
         Base.metadata.create_all(engine)
@@ -93,39 +74,31 @@
             data.append(line.to_dict())
         session.bulk_insert_mappings(sql_class, data)
         session.commit()
         session.close()
 
         metadata = MetaData()
         metadata.reflect(bind=engine)
-        sql_table = Table(
-            input_class_name.lower(), metadata, autoload=True, autoload_with=engine
-        )
-
-        template_table = "\nOnly use the following tables:\n" + str(
-            CreateTable(sql_table).compile(engine)
-        )
+        sql_table = Table(input_class_name.lower(), metadata, autoload=True, autoload_with=engine)
+
+        template_table = "\nOnly use the following tables:\n" + str(CreateTable(sql_table).compile(engine))
         # If the table isn't too large, would be better to also include example data
         template_start = """Given an input question, first create a syntactically correct {dialect} query to run, then look at the results of the query and return the answer. Use the following format:
 
         Question: "Question here"
         SQLQuery: "SQL Query to run"
         SQLResult: "Result of the SQLQuery"
         Answer: "Final answer here"
         """
         template_end = "Question: {input}"
 
         prompt_template = template_start + template_table + template_end
 
-        prompt = PromptTemplate(
-            input_variables=["input", "dialect"], template=prompt_template
-        )
+        prompt = PromptTemplate(input_variables=["input", "dialect"], template=prompt_template)
         db = SQLDatabase.from_uri(f"sqlite:///{input_class_name.lower()}.db")
-        db_chain = SQLDatabaseChain.from_llm(
-            llm=self.llm, db=db, prompt=prompt, verbose=True
-        )
+        db_chain = SQLDatabaseChain.from_llm(llm=self.llm, db=db, prompt=prompt, verbose=True)
         res = db_chain.run(query)
 
         # Drop the created table so it doesn't overwrite later
         sql_table.drop(engine)
 
         return res
```

