# Comparing `tmp/windmill_api-1.95.0.tar.gz` & `tmp/windmill_api-1.95.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.95.0.tar", max compression
+gzip compressed data, was "windmill_api-1.95.1.tar", max compression
```

## Comparing `windmill_api-1.95.0.tar` & `windmill_api-1.95.1.tar`

### file list

```diff
@@ -1,1289 +1,1289 @@
--rw-r--r--   0        0        0    11348 2023-05-05 21:28:18.692565 windmill_api-1.95.0/LICENSE
--rw-r--r--   0        0        0     2952 2023-05-05 21:28:18.700565 windmill_api-1.95.0/README.md
--rw-r--r--   0        0        0      717 2023-05-05 21:28:18.696565 windmill_api-1.95.0/pyproject.toml
--rw-r--r--   0        0        0      100 2023-05-05 21:27:47.100202 windmill_api-1.95.0/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-05-05 21:27:47.588208 windmill_api-1.95.0/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.692209 windmill_api-1.95.0/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-05-05 21:27:57.972350 windmill_api-1.95.0/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-05-05 21:27:57.968350 windmill_api-1.95.0/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-05-05 21:27:57.996350 windmill_api-1.95.0/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-05-05 21:27:58.024351 windmill_api-1.95.0/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-05-05 21:27:58.032351 windmill_api-1.95.0/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3187 2023-05-05 21:27:58.064351 windmill_api-1.95.0/windmill_api/api/app/get_app_by_path_with_draft.py
--rw-r--r--   0        0        0     3031 2023-05-05 21:27:58.072351 windmill_api-1.95.0/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-05-05 21:27:58.116351 windmill_api-1.95.0/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-05-05 21:27:58.124352 windmill_api-1.95.0/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-05-05 21:27:58.144352 windmill_api-1.95.0/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-05-05 21:27:58.212353 windmill_api-1.95.0/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-05-05 21:27:58.176352 windmill_api-1.95.0/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-05-05 21:27:58.208352 windmill_api-1.95.0/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.624208 windmill_api-1.95.0/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-05-05 21:27:58.248353 windmill_api-1.95.0/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-05-05 21:27:58.316354 windmill_api-1.95.0/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.768210 windmill_api-1.95.0/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-05-05 21:27:58.276353 windmill_api-1.95.0/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-05-05 21:27:58.300353 windmill_api-1.95.0/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-05-05 21:27:58.332354 windmill_api-1.95.0/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.724209 windmill_api-1.95.0/windmill_api/api/draft/__init__.py
--rw-r--r--   0        0        0     2019 2023-05-05 21:27:58.344354 windmill_api-1.95.0/windmill_api/api/draft/create_draft.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.772210 windmill_api-1.95.0/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-05-05 21:27:58.364354 windmill_api-1.95.0/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-05-05 21:27:58.376354 windmill_api-1.95.0/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.684209 windmill_api-1.95.0/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-05 21:27:58.392354 windmill_api-1.95.0/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-05-05 21:27:58.404355 windmill_api-1.95.0/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-05-05 21:27:58.420355 windmill_api-1.95.0/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-05-05 21:27:58.472355 windmill_api-1.95.0/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-05-05 21:27:58.472355 windmill_api-1.95.0/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     3205 2023-05-05 21:27:58.512356 windmill_api-1.95.0/windmill_api/api/flow/get_flow_by_path_with_draft.py
--rw-r--r--   0        0        0     4827 2023-05-05 21:27:58.528356 windmill_api-1.95.0/windmill_api/api/flow/get_flow_input_history_by_path.py
--rw-r--r--   0        0        0     2667 2023-05-05 21:27:58.548356 windmill_api-1.95.0/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-05-05 21:27:58.556356 windmill_api-1.95.0/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-05-05 21:27:58.648357 windmill_api-1.95.0/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-05-05 21:27:58.584356 windmill_api-1.95.0/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-05-05 21:27:58.616357 windmill_api-1.95.0/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.760210 windmill_api-1.95.0/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-05-05 21:27:58.644357 windmill_api-1.95.0/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-05-05 21:27:58.672357 windmill_api-1.95.0/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-05-05 21:27:58.676358 windmill_api-1.95.0/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-05-05 21:27:58.712358 windmill_api-1.95.0/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-05-05 21:27:58.716358 windmill_api-1.95.0/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-05-05 21:27:58.756358 windmill_api-1.95.0/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-05-05 21:27:58.772359 windmill_api-1.95.0/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-05-05 21:27:58.804359 windmill_api-1.95.0/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-05-05 21:27:58.840359 windmill_api-1.95.0/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.768210 windmill_api-1.95.0/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-05-05 21:27:58.836359 windmill_api-1.95.0/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-05-05 21:27:58.876360 windmill_api-1.95.0/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-05-05 21:27:58.872360 windmill_api-1.95.0/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.756210 windmill_api-1.95.0/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-05-05 21:27:58.908360 windmill_api-1.95.0/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-05-05 21:27:58.904360 windmill_api-1.95.0/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-05-05 21:27:58.932360 windmill_api-1.95.0/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-05-05 21:27:58.948360 windmill_api-1.95.0/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-05-05 21:27:58.976361 windmill_api-1.95.0/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-05-05 21:27:59.004361 windmill_api-1.95.0/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-05-05 21:27:59.004361 windmill_api-1.95.0/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-05-05 21:27:59.036361 windmill_api-1.95.0/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.772210 windmill_api-1.95.0/windmill_api/api/input_/__init__.py
--rw-r--r--   0        0        0     3338 2023-05-05 21:27:59.052362 windmill_api-1.95.0/windmill_api/api/input_/create_input.py
--rw-r--r--   0        0        0     1811 2023-05-05 21:27:59.060362 windmill_api-1.95.0/windmill_api/api/input_/delete_input.py
--rw-r--r--   0        0        0     6187 2023-05-05 21:27:59.140362 windmill_api-1.95.0/windmill_api/api/input_/get_input_history.py
--rw-r--r--   0        0        0     6010 2023-05-05 21:27:59.128362 windmill_api-1.95.0/windmill_api/api/input_/list_inputs.py
--rw-r--r--   0        0        0     2025 2023-05-05 21:27:59.176363 windmill_api-1.95.0/windmill_api/api/input_/update_input.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.724209 windmill_api-1.95.0/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-05 21:27:59.172363 windmill_api-1.95.0/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-05-05 21:27:59.212363 windmill_api-1.95.0/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-05 21:27:59.220363 windmill_api-1.95.0/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-05-05 21:27:59.248364 windmill_api-1.95.0/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-05-05 21:27:59.256364 windmill_api-1.95.0/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-05-05 21:27:59.276364 windmill_api-1.95.0/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-05-05 21:27:59.296364 windmill_api-1.95.0/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-05-05 21:27:59.300364 windmill_api-1.95.0/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-05-05 21:27:59.336365 windmill_api-1.95.0/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-05-05 21:27:59.356365 windmill_api-1.95.0/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-05-05 21:27:59.392365 windmill_api-1.95.0/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-05-05 21:27:59.408365 windmill_api-1.95.0/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    13065 2023-05-05 21:27:59.556367 windmill_api-1.95.0/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    12292 2023-05-05 21:27:59.564367 windmill_api-1.95.0/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12830 2023-05-05 21:27:59.704368 windmill_api-1.95.0/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-05-05 21:27:59.592367 windmill_api-1.95.0/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-05-05 21:27:59.620368 windmill_api-1.95.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2994 2023-05-05 21:27:59.660368 windmill_api-1.95.0/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-05 21:27:59.704368 windmill_api-1.95.0/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-05-05 21:27:59.756369 windmill_api-1.95.0/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-05-05 21:27:59.744369 windmill_api-1.95.0/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-05-05 21:27:59.800370 windmill_api-1.95.0/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-05-05 21:27:59.832370 windmill_api-1.95.0/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-05-05 21:27:59.840370 windmill_api-1.95.0/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     3215 2023-05-05 21:27:59.872370 windmill_api-1.95.0/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     3521 2023-05-05 21:27:59.912371 windmill_api-1.95.0/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0     3356 2023-05-05 21:27:59.920371 windmill_api-1.95.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.656209 windmill_api-1.95.0/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-05 21:27:59.952371 windmill_api-1.95.0/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-05-05 21:27:59.944371 windmill_api-1.95.0/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-05-05 21:27:59.972371 windmill_api-1.95.0/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-05-05 21:27:59.980372 windmill_api-1.95.0/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-05-05 21:28:00.000372 windmill_api-1.95.0/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-05-05 21:28:00.016372 windmill_api-1.95.0/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-05-05 21:28:00.032372 windmill_api-1.95.0/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-05-05 21:28:00.052372 windmill_api-1.95.0/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.660209 windmill_api-1.95.0/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-05 21:28:00.060372 windmill_api-1.95.0/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-05-05 21:28:00.080373 windmill_api-1.95.0/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-05-05 21:28:00.088373 windmill_api-1.95.0/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-05-05 21:28:00.108373 windmill_api-1.95.0/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-05-05 21:28:00.124373 windmill_api-1.95.0/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-05-05 21:28:00.148373 windmill_api-1.95.0/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-05-05 21:28:00.176374 windmill_api-1.95.0/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-05-05 21:28:00.188374 windmill_api-1.95.0/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-05-05 21:28:00.204374 windmill_api-1.95.0/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-05-05 21:28:00.276375 windmill_api-1.95.0/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-05-05 21:28:00.244374 windmill_api-1.95.0/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-05-05 21:28:00.280375 windmill_api-1.95.0/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-05-05 21:28:00.308375 windmill_api-1.95.0/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-05-05 21:28:00.308375 windmill_api-1.95.0/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-05-05 21:28:00.340375 windmill_api-1.95.0/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.752210 windmill_api-1.95.0/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-05 21:28:00.336375 windmill_api-1.95.0/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-05-05 21:28:00.360376 windmill_api-1.95.0/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-05-05 21:28:00.380376 windmill_api-1.95.0/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-05-05 21:28:00.400376 windmill_api-1.95.0/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-05-05 21:28:00.436376 windmill_api-1.95.0/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-05-05 21:28:00.440376 windmill_api-1.95.0/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-05-05 21:28:00.464377 windmill_api-1.95.0/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-05-05 21:28:00.484377 windmill_api-1.95.0/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.668209 windmill_api-1.95.0/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-05-05 21:28:00.508377 windmill_api-1.95.0/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-05-05 21:28:00.512377 windmill_api-1.95.0/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-05 21:28:00.544378 windmill_api-1.95.0/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-05-05 21:28:00.540377 windmill_api-1.95.0/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-05-05 21:28:00.576378 windmill_api-1.95.0/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-05-05 21:28:00.604378 windmill_api-1.95.0/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-05 21:28:00.612378 windmill_api-1.95.0/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-05-05 21:28:00.644379 windmill_api-1.95.0/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-05-05 21:28:00.652379 windmill_api-1.95.0/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-05-05 21:28:00.672379 windmill_api-1.95.0/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-05-05 21:28:00.688379 windmill_api-1.95.0/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-05-05 21:28:00.712379 windmill_api-1.95.0/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3241 2023-05-05 21:28:00.728380 windmill_api-1.95.0/windmill_api/api/script/get_script_by_path_with_draft.py
--rw-r--r--   0        0        0     3276 2023-05-05 21:28:00.752380 windmill_api-1.95.0/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-05-05 21:28:00.764380 windmill_api-1.95.0/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-05-05 21:28:00.788380 windmill_api-1.95.0/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-05-05 21:28:00.804380 windmill_api-1.95.0/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-05-05 21:28:00.936382 windmill_api-1.95.0/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-05-05 21:28:00.840381 windmill_api-1.95.0/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-05-05 21:28:00.864381 windmill_api-1.95.0/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-05-05 21:28:00.892381 windmill_api-1.95.0/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0     2119 2023-05-05 21:28:00.920382 windmill_api-1.95.0/windmill_api/api/script/raw_script_by_path_tokened.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.600208 windmill_api-1.95.0/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-05-05 21:28:00.944382 windmill_api-1.95.0/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-05-05 21:28:00.960382 windmill_api-1.95.0/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.628208 windmill_api-1.95.0/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-05-05 21:28:00.976382 windmill_api-1.95.0/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-05-05 21:28:00.984382 windmill_api-1.95.0/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     1991 2023-05-05 21:28:01.004382 windmill_api-1.95.0/windmill_api/api/user/create_token_impersonate.py
--rw-r--r--   0        0        0     2058 2023-05-05 21:28:01.012383 windmill_api-1.95.0/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-05-05 21:28:01.032383 windmill_api-1.95.0/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-05-05 21:28:01.036383 windmill_api-1.95.0/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-05-05 21:28:01.056383 windmill_api-1.95.0/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-05-05 21:28:01.064383 windmill_api-1.95.0/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-05-05 21:28:01.080383 windmill_api-1.95.0/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-05-05 21:28:01.084383 windmill_api-1.95.0/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-05-05 21:28:01.108384 windmill_api-1.95.0/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-05-05 21:28:01.120384 windmill_api-1.95.0/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-05-05 21:28:01.156384 windmill_api-1.95.0/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-05-05 21:28:01.168384 windmill_api-1.95.0/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-05-05 21:28:01.180384 windmill_api-1.95.0/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-05-05 21:28:01.204385 windmill_api-1.95.0/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-05-05 21:28:01.216385 windmill_api-1.95.0/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-05-05 21:28:01.244385 windmill_api-1.95.0/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-05-05 21:28:01.268385 windmill_api-1.95.0/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-05-05 21:28:01.300386 windmill_api-1.95.0/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-05-05 21:28:01.292386 windmill_api-1.95.0/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-05-05 21:28:01.320386 windmill_api-1.95.0/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-05-05 21:28:01.324386 windmill_api-1.95.0/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-05-05 21:28:01.344386 windmill_api-1.95.0/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-05-05 21:28:01.356386 windmill_api-1.95.0/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-05-05 21:28:01.380386 windmill_api-1.95.0/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-05-05 21:28:01.396387 windmill_api-1.95.0/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.652208 windmill_api-1.95.0/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-05-05 21:28:01.420387 windmill_api-1.95.0/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-05-05 21:28:01.420387 windmill_api-1.95.0/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-05-05 21:28:01.480388 windmill_api-1.95.0/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-05-05 21:28:01.468387 windmill_api-1.95.0/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-05-05 21:28:01.508388 windmill_api-1.95.0/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-05-05 21:28:01.520388 windmill_api-1.95.0/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-05-05 21:28:01.544388 windmill_api-1.95.0/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.724209 windmill_api-1.95.0/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     2448 2023-05-05 21:28:01.556388 windmill_api-1.95.0/windmill_api/api/worker/get_custom_tags.py
--rw-r--r--   0        0        0     3896 2023-05-05 21:28:01.608389 windmill_api-1.95.0/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-05-05 21:27:47.640208 windmill_api-1.95.0/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-05-05 21:28:01.584389 windmill_api-1.95.0/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-05-05 21:28:01.604389 windmill_api-1.95.0/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-05-05 21:28:01.636389 windmill_api-1.95.0/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-05-05 21:28:01.644389 windmill_api-1.95.0/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-05-05 21:28:01.660390 windmill_api-1.95.0/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-05-05 21:28:01.672390 windmill_api-1.95.0/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-05-05 21:28:01.684390 windmill_api-1.95.0/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-05-05 21:28:01.700390 windmill_api-1.95.0/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-05-05 21:28:01.716390 windmill_api-1.95.0/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-05-05 21:28:01.724390 windmill_api-1.95.0/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-05-05 21:28:01.748391 windmill_api-1.95.0/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-05-05 21:28:01.764391 windmill_api-1.95.0/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-05-05 21:28:01.772391 windmill_api-1.95.0/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-05-05 21:28:01.796391 windmill_api-1.95.0/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-05-05 21:28:01.832391 windmill_api-1.95.0/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-05-05 21:28:01.828391 windmill_api-1.95.0/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-05-05 21:28:01.864392 windmill_api-1.95.0/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-05-05 21:28:01.884392 windmill_api-1.95.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-05-05 21:28:01.888392 windmill_api-1.95.0/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-05-05 21:28:01.912392 windmill_api-1.95.0/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-05-05 21:28:18.692565 windmill_api-1.95.0/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-05 21:28:01.940393 windmill_api-1.95.0/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-05-05 21:28:01.964393 windmill_api-1.95.0/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      301 2023-05-05 21:27:56.536335 windmill_api-1.95.0/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-05-05 21:28:01.996393 windmill_api-1.95.0/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-05-05 21:28:02.024393 windmill_api-1.95.0/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-05-05 21:28:02.044394 windmill_api-1.95.0/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-05-05 21:28:02.076394 windmill_api-1.95.0/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-05-05 21:27:57.040340 windmill_api-1.95.0/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-05-05 21:28:02.068394 windmill_api-1.95.0/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-05-05 21:28:02.112394 windmill_api-1.95.0/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-05-05 21:27:57.088340 windmill_api-1.95.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-05-05 21:28:02.104394 windmill_api-1.95.0/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-05-05 21:28:02.124395 windmill_api-1.95.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4638 2023-05-05 21:28:02.168395 windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft.py
--rw-r--r--   0        0        0      220 2023-05-05 21:27:57.104341 windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
--rw-r--r--   0        0        0     1284 2023-05-05 21:28:02.148395 windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
--rw-r--r--   0        0        0     3828 2023-05-05 21:28:02.224396 windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft_policy.py
--rw-r--r--   0        0        0      226 2023-05-05 21:27:56.644336 windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
--rw-r--r--   0        0        0     2020 2023-05-05 21:28:02.192395 windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
--rw-r--r--   0        0        0     1417 2023-05-05 21:28:02.212396 windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1569 2023-05-05 21:28:02.260396 windmill_api-1.95.0/windmill_api/models/archive_flow_by_path_json_body.py
--rw-r--r--   0        0        0     7662 2023-05-05 21:28:02.320397 windmill_api-1.95.0/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-05-05 21:28:02.276396 windmill_api-1.95.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-05-05 21:27:57.324343 windmill_api-1.95.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-05-05 21:27:57.008340 windmill_api-1.95.0/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-05-05 21:28:02.300396 windmill_api-1.95.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-05-05 21:28:02.348397 windmill_api-1.95.0/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-05-05 21:27:57.076340 windmill_api-1.95.0/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-05-05 21:27:56.968339 windmill_api-1.95.0/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-05-05 21:28:02.344397 windmill_api-1.95.0/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-05-05 21:28:02.384397 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-05 21:28:02.404398 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-05 21:27:56.984339 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-05 21:28:02.412398 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-05 21:28:02.428398 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-05 21:28:02.440398 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-05 21:28:02.464398 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-05 21:27:57.148341 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-05 21:28:02.468398 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-05 21:28:02.500398 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-05 21:27:57.088340 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-05 21:28:02.492398 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-05 21:27:56.380333 windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-05-05 21:28:02.528399 windmill_api-1.95.0/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-05-05 21:28:02.536399 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-05 21:28:02.636400 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-05 21:28:02.572399 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-05 21:28:02.620400 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-05 21:28:02.652400 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-05 21:28:02.668400 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-05 21:27:57.060340 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-05 21:28:02.680400 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-05 21:27:56.656336 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-05 21:28:02.700401 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-05 21:28:02.708401 windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-05 21:27:56.580335 windmill_api-1.95.0/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-05-05 21:28:02.740401 windmill_api-1.95.0/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-05-05 21:28:02.744401 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-05 21:28:02.820402 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-05 21:28:02.780402 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-05 21:28:02.812402 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-05 21:28:02.844402 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-05 21:28:02.844402 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-05 21:27:56.976339 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-05 21:28:02.872403 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-05 21:27:56.520334 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-05 21:28:02.876402 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-05 21:28:02.900403 windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-05 21:28:02.956403 windmill_api-1.95.0/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-05-05 21:28:02.960404 windmill_api-1.95.0/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-05 21:28:03.008404 windmill_api-1.95.0/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-05 21:28:02.988404 windmill_api-1.95.0/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-05 21:28:03.020404 windmill_api-1.95.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-05 21:27:56.656336 windmill_api-1.95.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-05 21:28:03.036404 windmill_api-1.95.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-05 21:27:57.236342 windmill_api-1.95.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-05 21:28:03.052404 windmill_api-1.95.0/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-05 21:28:03.064405 windmill_api-1.95.0/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-05 21:27:57.068340 windmill_api-1.95.0/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-05-05 21:28:03.080405 windmill_api-1.95.0/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-05 21:28:03.084405 windmill_api-1.95.0/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10508 2023-05-05 21:28:03.212406 windmill_api-1.95.0/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-05-05 21:28:03.100405 windmill_api-1.95.0/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-05-05 21:28:03.144405 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-05-05 21:28:03.224406 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-05-05 21:28:03.248407 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-05-05 21:28:03.256407 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-05-05 21:27:57.248342 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-05-05 21:28:03.272407 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-05-05 21:28:03.292407 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-05-05 21:27:56.504334 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-05-05 21:28:03.388408 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-05-05 21:28:03.320407 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-05-05 21:28:03.372408 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-05-05 21:27:56.264332 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-05-05 21:28:03.396408 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-05-05 21:28:03.424409 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-05-05 21:27:57.324343 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-05-05 21:28:03.432409 windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-05-05 21:27:56.740337 windmill_api-1.95.0/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-05-05 21:27:56.252332 windmill_api-1.95.0/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-05-05 21:28:03.468409 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-05-05 21:28:03.508409 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-05-05 21:28:03.508409 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-05-05 21:28:03.536410 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-05 21:28:03.544410 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-05 21:28:03.564410 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-05 21:27:56.832338 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-05 21:28:03.576410 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-05 21:27:56.828338 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-05 21:28:03.596410 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-05 21:28:03.604411 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-05-05 21:28:03.672411 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-05-05 21:28:03.644411 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-05-05 21:28:03.672411 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-05-05 21:28:03.724412 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-05-05 21:28:03.732412 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-05-05 21:27:56.624335 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-05-05 21:28:03.752412 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-05-05 21:27:56.664336 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-05-05 21:28:03.764412 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-05-05 21:28:03.780412 windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-05-05 21:28:03.788412 windmill_api-1.95.0/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-05-05 21:28:03.816413 windmill_api-1.95.0/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-05-05 21:28:03.816413 windmill_api-1.95.0/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-05-05 21:28:03.840413 windmill_api-1.95.0/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-05-05 21:28:03.848413 windmill_api-1.95.0/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2367 2023-05-05 21:28:03.880413 windmill_api-1.95.0/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-05 21:28:03.892413 windmill_api-1.95.0/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-05 21:27:57.328343 windmill_api-1.95.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-05 21:28:03.904414 windmill_api-1.95.0/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-05 21:28:03.912414 windmill_api-1.95.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1947 2023-05-05 21:28:03.940414 windmill_api-1.95.0/windmill_api/models/create_draft_json_body.py
--rw-r--r--   0        0        0      183 2023-05-05 21:27:56.784337 windmill_api-1.95.0/windmill_api/models/create_draft_json_body_typ.py
--rw-r--r--   0        0        0     1550 2023-05-05 21:28:03.936414 windmill_api-1.95.0/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     2126 2023-05-05 21:28:03.972414 windmill_api-1.95.0/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-05-05 21:28:03.968414 windmill_api-1.95.0/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     1613 2023-05-05 21:28:03.996415 windmill_api-1.95.0/windmill_api/models/create_input.py
--rw-r--r--   0        0        0     1171 2023-05-05 21:28:03.988415 windmill_api-1.95.0/windmill_api/models/create_input_args.py
--rw-r--r--   0        0        0     1701 2023-05-05 21:28:04.016415 windmill_api-1.95.0/windmill_api/models/create_input_json_body.py
--rw-r--r--   0        0        0     1217 2023-05-05 21:28:04.016415 windmill_api-1.95.0/windmill_api/models/create_input_json_body_args.py
--rw-r--r--   0        0        0      214 2023-05-05 21:27:56.280332 windmill_api-1.95.0/windmill_api/models/create_input_runnable_type.py
--rw-r--r--   0        0        0     2094 2023-05-05 21:28:04.048415 windmill_api-1.95.0/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-05-05 21:28:04.048415 windmill_api-1.95.0/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-05-05 21:28:04.104416 windmill_api-1.95.0/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2780 2023-05-05 21:28:04.108416 windmill_api-1.95.0/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-05 21:28:04.124416 windmill_api-1.95.0/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     5120 2023-05-05 21:28:04.192417 windmill_api-1.95.0/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-05-05 21:27:57.328343 windmill_api-1.95.0/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-05-05 21:27:56.256332 windmill_api-1.95.0/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-05-05 21:28:04.148416 windmill_api-1.95.0/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2534 2023-05-05 21:28:04.184417 windmill_api-1.95.0/windmill_api/models/create_token_impersonate_json_body.py
--rw-r--r--   0        0        0     2169 2023-05-05 21:28:04.216417 windmill_api-1.95.0/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-05-05 21:28:04.228417 windmill_api-1.95.0/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-05-05 21:28:04.244417 windmill_api-1.95.0/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-05-05 21:28:04.268417 windmill_api-1.95.0/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-05-05 21:28:04.280418 windmill_api-1.95.0/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-05-05 21:28:04.296418 windmill_api-1.95.0/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-05-05 21:28:04.308418 windmill_api-1.95.0/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-05-05 21:28:04.320418 windmill_api-1.95.0/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    11110 2023-05-05 21:28:04.464420 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-05-05 21:28:04.340418 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-05-05 21:28:04.380419 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-05-05 21:28:04.492420 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-05-05 21:28:04.488420 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-05-05 21:28:04.516420 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-05-05 21:27:56.860338 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-05-05 21:28:04.520420 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-05-05 21:28:04.552420 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-05-05 21:27:57.064340 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-05-05 21:28:04.604421 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-05-05 21:28:04.576421 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-05-05 21:28:04.604421 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-05-05 21:27:56.424333 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-05-05 21:28:04.632421 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-05-05 21:28:04.644421 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-05-05 21:27:56.440333 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-05-05 21:28:04.664422 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-05-05 21:27:56.260332 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-05-05 21:27:56.800337 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-05-05 21:28:04.688422 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-05-05 21:28:04.744423 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-05-05 21:28:04.728422 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-05-05 21:28:04.756423 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-05-05 21:28:04.776423 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-05-05 21:28:04.788423 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-05-05 21:27:56.452334 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-05 21:28:04.832424 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-05-05 21:27:57.052340 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-05-05 21:28:04.816423 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-05-05 21:28:04.868424 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-05-05 21:28:04.912424 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-05-05 21:28:04.908424 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-05-05 21:28:04.936425 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-05-05 21:28:04.944425 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-05-05 21:28:04.964425 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-05 21:27:57.032340 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-05-05 21:28:04.972425 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-05 21:27:56.848338 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-05-05 21:28:04.996425 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-05-05 21:28:05.000425 windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-05-05 21:28:05.024426 windmill_api-1.95.0/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     7636 2023-05-05 21:28:05.088426 windmill_api-1.95.0/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-05-05 21:28:05.044426 windmill_api-1.95.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-05-05 21:27:56.860338 windmill_api-1.95.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-05-05 21:27:56.340332 windmill_api-1.95.0/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-05-05 21:28:05.068426 windmill_api-1.95.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-05-05 21:28:05.108426 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-05 21:28:05.148427 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-05 21:27:56.436334 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-05 21:28:05.136427 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-05 21:28:05.160427 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-05 21:28:05.204427 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-05 21:28:05.200427 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-05 21:27:56.848338 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-05 21:28:05.244428 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-05 21:28:05.240428 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-05 21:27:56.768337 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-05 21:28:05.264428 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-05 21:27:56.620335 windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-05-05 21:28:05.272428 windmill_api-1.95.0/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-05-05 21:28:05.296428 windmill_api-1.95.0/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-05-05 21:28:05.300428 windmill_api-1.95.0/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1845 2023-05-05 21:28:05.324429 windmill_api-1.95.0/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-05-05 21:28:05.320429 windmill_api-1.95.0/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-05-05 21:28:05.348429 windmill_api-1.95.0/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-05-05 21:28:05.364429 windmill_api-1.95.0/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-05-05 21:28:05.368429 windmill_api-1.95.0/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-05-05 21:28:05.396429 windmill_api-1.95.0/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-05-05 21:28:05.420430 windmill_api-1.95.0/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-05-05 21:28:05.428430 windmill_api-1.95.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-05-05 21:28:05.448430 windmill_api-1.95.0/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-05-05 21:28:05.452430 windmill_api-1.95.0/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-05-05 21:28:05.468430 windmill_api-1.95.0/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4924 2023-05-05 21:28:05.520431 windmill_api-1.95.0/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-05-05 21:28:05.488430 windmill_api-1.95.0/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3707 2023-05-05 21:28:05.540431 windmill_api-1.95.0/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-05-05 21:28:05.544431 windmill_api-1.95.0/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-05-05 21:28:05.644432 windmill_api-1.95.0/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-05-05 21:28:05.580431 windmill_api-1.95.0/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-05-05 21:28:05.632432 windmill_api-1.95.0/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-05-05 21:28:05.664432 windmill_api-1.95.0/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-05-05 21:28:05.672432 windmill_api-1.95.0/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-05-05 21:27:56.872338 windmill_api-1.95.0/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-05-05 21:28:05.692432 windmill_api-1.95.0/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-05-05 21:27:56.564335 windmill_api-1.95.0/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-05-05 21:28:05.700433 windmill_api-1.95.0/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-05-05 21:28:05.716433 windmill_api-1.95.0/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3292 2023-05-05 21:28:05.756433 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-05-05 21:28:05.752433 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-05 21:28:05.780434 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-05 21:27:56.852338 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-05 21:28:05.784433 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-05 21:27:56.864338 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-05-05 21:27:56.652336 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-05-05 21:27:57.224342 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-05-05 21:28:05.820434 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-05-05 21:28:05.824434 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-05 21:28:05.848434 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-05 21:27:57.300343 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-05 21:28:05.852434 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-05 21:27:57.116341 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-05-05 21:27:56.528334 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-05-05 21:28:05.880435 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-05-05 21:28:05.888435 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-05 21:28:05.908435 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-05 21:27:57.164341 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-05 21:28:05.920435 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-05 21:27:57.156341 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-05-05 21:27:56.520334 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-05-05 21:28:05.992436 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-05-05 21:28:05.948435 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-05-05 21:27:56.716336 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-05-05 21:28:05.976436 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-05-05 21:27:57.224342 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-05-05 21:28:06.080437 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-05-05 21:28:06.032436 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-05 21:28:06.060436 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-05 21:28:06.092437 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-05 21:28:06.108437 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-05 21:27:57.308343 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-05 21:28:06.120437 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-05 21:27:56.252332 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-05 21:28:06.136437 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-05 21:28:06.148437 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-05-05 21:27:56.664336 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-05-05 21:28:06.176438 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-05-05 21:28:06.180438 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-05 21:28:06.260439 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-05 21:28:06.220438 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-05 21:28:06.244438 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-05 21:28:06.280439 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-05 21:28:06.288439 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-05 21:27:56.680336 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-05 21:28:06.336439 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-05 21:27:56.552335 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-05 21:28:06.316439 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-05 21:28:06.376440 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-05-05 21:28:06.416440 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-05-05 21:28:06.420440 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-05 21:28:06.440440 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-05 21:28:06.452441 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-05 21:28:06.468441 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-05 21:27:56.324332 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-05 21:28:06.480441 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-05 21:27:56.432333 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-05 21:28:06.500441 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-05 21:28:06.512441 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-05 21:27:56.328332 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-05-05 21:28:06.536441 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-05-05 21:28:06.548442 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-05 21:28:06.620442 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-05 21:28:06.584442 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-05 21:28:06.612442 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-05 21:28:06.644442 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-05 21:28:06.648443 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-05 21:27:56.492334 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-05 21:28:06.672443 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-05 21:27:56.796337 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-05 21:28:06.720443 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-05 21:28:06.700443 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-05 21:27:56.996339 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-05-05 21:28:06.752444 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-05-05 21:27:57.180341 windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-05-05 21:28:06.752444 windmill_api-1.95.0/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-05-05 21:28:06.768444 windmill_api-1.95.0/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-05-05 21:28:06.796444 windmill_api-1.95.0/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-05-05 21:28:06.848445 windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-05-05 21:28:06.832445 windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-05-05 21:28:06.860445 windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-05-05 21:28:06.876445 windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-05-05 21:28:06.892445 windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-05 21:27:56.872338 windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-05-05 21:28:06.904445 windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-05 21:27:56.376333 windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-05-05 21:28:06.920445 windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-05-05 21:28:06.932446 windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-05-05 21:28:07.004446 windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-05-05 21:28:06.972446 windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-05-05 21:28:07.000446 windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-05-05 21:28:07.032446 windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-05-05 21:28:07.032446 windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-05 21:27:56.472334 windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-05-05 21:28:07.056447 windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-05 21:27:56.392333 windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-05-05 21:28:07.064447 windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-05-05 21:28:07.116448 windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-05-05 21:28:07.132448 windmill_api-1.95.0/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-05-05 21:28:07.156448 windmill_api-1.95.0/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-05-05 21:28:07.216448 windmill_api-1.95.0/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-05-05 21:28:07.180448 windmill_api-1.95.0/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-05-05 21:28:07.208449 windmill_api-1.95.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-05-05 21:27:56.440333 windmill_api-1.95.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-05-05 21:28:07.236449 windmill_api-1.95.0/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-05-05 21:28:07.252449 windmill_api-1.95.0/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-05-05 21:27:57.064340 windmill_api-1.95.0/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-05-05 21:28:07.312450 windmill_api-1.95.0/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-05-05 21:28:07.276449 windmill_api-1.95.0/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-05-05 21:28:07.304449 windmill_api-1.95.0/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-05-05 21:27:57.120341 windmill_api-1.95.0/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-05-05 21:28:07.344450 windmill_api-1.95.0/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-05-05 21:28:07.348450 windmill_api-1.95.0/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-05-05 21:27:57.148341 windmill_api-1.95.0/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-05-05 21:28:07.452451 windmill_api-1.95.0/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-05-05 21:28:07.400450 windmill_api-1.95.0/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-05-05 21:28:07.432451 windmill_api-1.95.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-05-05 21:27:56.780337 windmill_api-1.95.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-05-05 21:28:07.460451 windmill_api-1.95.0/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-05-05 21:28:07.528452 windmill_api-1.95.0/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-05-05 21:27:56.632336 windmill_api-1.95.0/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-05-05 21:28:07.492451 windmill_api-1.95.0/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-05-05 21:28:07.576452 windmill_api-1.95.0/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-05-05 21:28:07.608453 windmill_api-1.95.0/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-05-05 21:28:07.612453 windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-05-05 21:28:07.636453 windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-05 21:28:07.644453 windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-05 21:28:07.664453 windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-05 21:27:56.808338 windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-05 21:28:07.676453 windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-05 21:27:57.032340 windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-05 21:28:07.692453 windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-05 21:28:07.704454 windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-05 21:28:07.768454 windmill_api-1.95.0/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-05-05 21:28:07.744454 windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-05 21:28:07.772454 windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-05 21:28:07.800455 windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-05 21:28:07.804455 windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-05 21:27:56.632336 windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-05 21:28:07.828455 windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-05 21:27:56.828338 windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-05 21:28:07.832455 windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-05 21:28:07.892456 windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-05-05 21:28:07.860455 windmill_api-1.95.0/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-05-05 21:28:07.880455 windmill_api-1.95.0/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-05-05 21:28:07.908456 windmill_api-1.95.0/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-05-05 21:28:07.940456 windmill_api-1.95.0/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-05-05 21:28:07.972456 windmill_api-1.95.0/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-05-05 21:27:56.996339 windmill_api-1.95.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-05-05 21:28:07.968456 windmill_api-1.95.0/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-05-05 21:27:56.872338 windmill_api-1.95.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-05-05 21:28:08.048457 windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-05-05 21:28:08.012457 windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-05-05 21:28:08.040457 windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-05 21:28:08.072457 windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-05 21:28:08.076458 windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-05 21:27:56.288332 windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-05 21:28:08.100458 windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-05 21:27:57.248342 windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-05 21:28:08.104458 windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-05 21:28:08.128458 windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-05-05 21:27:56.472334 windmill_api-1.95.0/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-05-05 21:28:08.160458 windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-05-05 21:27:57.272342 windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-05-05 21:28:08.148458 windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-05-05 21:28:08.192459 windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-05-05 21:27:56.656336 windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-05-05 21:28:08.184459 windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-05-05 21:28:08.204459 windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4819 2023-05-05 21:28:08.288460 windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0      228 2023-05-05 21:27:57.108341 windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
--rw-r--r--   0        0        0     1330 2023-05-05 21:28:08.228459 windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
--rw-r--r--   0        0        0     3992 2023-05-05 21:28:08.272460 windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
--rw-r--r--   0        0        0      234 2023-05-05 21:27:56.688336 windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2160 2023-05-05 21:28:08.300460 windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1463 2023-05-05 21:28:08.308460 windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-05-05 21:28:08.392461 windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-05-05 21:27:56.724336 windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-05-05 21:28:08.328460 windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-05-05 21:28:08.380461 windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-05-05 21:27:57.036340 windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-05-05 21:28:08.404461 windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-05-05 21:28:08.412461 windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-05-05 21:28:08.452461 windmill_api-1.95.0/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-05-05 21:27:56.880338 windmill_api-1.95.0/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-05-05 21:27:57.168341 windmill_api-1.95.0/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-05-05 21:28:08.436461 windmill_api-1.95.0/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    11008 2023-05-05 21:28:08.572463 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-05-05 21:28:08.468462 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-05-05 21:28:08.516462 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-05-05 21:28:08.600463 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-05-05 21:28:08.596463 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-05-05 21:28:08.628463 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-05-05 21:27:56.528334 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-05-05 21:28:08.668464 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-05-05 21:28:08.660464 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-05-05 21:27:56.256332 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-05-05 21:28:08.804465 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-05-05 21:28:08.692464 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-05 21:28:08.724464 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-05 21:27:56.764337 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-05 21:28:08.752465 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-05 21:28:08.784465 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-05-05 21:27:56.528334 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-05-05 21:28:08.820465 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-05-05 21:27:56.544335 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-05-05 21:27:56.704336 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-05-05 21:28:08.848466 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-05-05 21:28:08.900466 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-05-05 21:28:08.888466 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-05-05 21:28:08.916466 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-05-05 21:28:08.932466 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-05-05 21:28:08.944467 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-05-05 21:27:56.552335 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-05-05 21:28:08.960467 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-05-05 21:27:57.192342 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-05-05 21:28:08.976467 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-05-05 21:28:08.984467 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-05-05 21:28:09.056468 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-05-05 21:28:09.060468 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-05-05 21:28:09.084468 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-05 21:28:09.092468 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-05 21:28:09.164469 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-05 21:27:56.856338 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-05 21:28:09.120468 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-05 21:27:56.728337 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-05 21:28:09.148469 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-05 21:28:09.176469 windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5374 2023-05-05 21:28:09.236470 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-05-05 21:28:09.196469 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-05-05 21:28:09.212469 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-05-05 21:28:09.256470 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-05-05 21:28:09.316470 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-05-05 21:28:09.292470 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-05-05 21:28:09.320470 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-05 21:28:09.348471 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-05 21:28:09.348471 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-05 21:27:56.236331 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-05 21:28:09.376471 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-05 21:27:56.304332 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-05 21:28:09.412471 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-05 21:28:09.404471 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-05-05 21:28:09.484472 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-05-05 21:28:09.452472 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-05-05 21:28:09.480472 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-05-05 21:28:09.512472 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-05-05 21:28:09.560473 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-05 21:27:56.248331 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-05-05 21:28:09.552473 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-05 21:27:56.656336 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-05-05 21:28:09.584473 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-05-05 21:28:09.584473 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2093 2023-05-05 21:28:09.612474 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5695 2023-05-05 21:28:09.652474 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0     1360 2023-05-05 21:28:09.632474 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
--rw-r--r--   0        0        0     1337 2023-05-05 21:28:09.652474 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0     3559 2023-05-05 21:28:09.692474 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
--rw-r--r--   0        0        0     7829 2023-05-05 21:28:09.732475 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
--rw-r--r--   0        0        0     3606 2023-05-05 21:28:09.732475 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
--rw-r--r--   0        0        0     2067 2023-05-05 21:28:09.760475 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2371 2023-05-05 21:28:09.768475 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2343 2023-05-05 21:28:09.788475 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      205 2023-05-05 21:27:56.468334 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2210 2023-05-05 21:28:09.796476 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      205 2023-05-05 21:27:56.568335 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2060 2023-05-05 21:28:09.816476 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2111 2023-05-05 21:28:09.824476 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7685 2023-05-05 21:28:09.928477 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
--rw-r--r--   0        0        0     3542 2023-05-05 21:28:09.860476 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
--rw-r--r--   0        0        0     2057 2023-05-05 21:28:09.940477 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2361 2023-05-05 21:28:09.960477 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2323 2023-05-05 21:28:09.968477 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      203 2023-05-05 21:27:56.420333 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2190 2023-05-05 21:28:09.988478 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      203 2023-05-05 21:27:57.296343 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2050 2023-05-05 21:28:10.000478 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2101 2023-05-05 21:28:10.020478 windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2756 2023-05-05 21:28:10.032478 windmill_api-1.95.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
--rw-r--r--   0        0        0     1337 2023-05-05 21:28:10.036478 windmill_api-1.95.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
--rw-r--r--   0        0        0     2010 2023-05-05 21:28:10.064478 windmill_api-1.95.0/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-05-05 21:28:10.056478 windmill_api-1.95.0/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-05-05 21:28:10.092479 windmill_api-1.95.0/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      301 2023-05-05 21:27:56.476334 windmill_api-1.95.0/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-05-05 21:28:10.084478 windmill_api-1.95.0/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-05-05 21:28:10.128479 windmill_api-1.95.0/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-05-05 21:28:10.112479 windmill_api-1.95.0/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-05-05 21:28:10.136479 windmill_api-1.95.0/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-05-05 21:28:10.152479 windmill_api-1.95.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-05-05 21:28:10.168479 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-05-05 21:28:10.188480 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-05-05 21:28:10.188480 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-05-05 21:28:10.264480 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-05-05 21:28:10.324481 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-05-05 21:28:10.300481 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-05-05 21:28:10.328481 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-05-05 21:28:10.356481 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-05-05 21:28:10.356481 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-05 21:27:57.028340 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-05-05 21:28:10.384482 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-05 21:27:56.528334 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-05-05 21:28:10.388482 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-05-05 21:28:10.412482 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-05-05 21:28:10.468483 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-05-05 21:28:10.448482 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-05-05 21:28:10.476483 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-05-05 21:28:10.500483 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-05-05 21:28:10.504483 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-05-05 21:27:57.336343 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-05-05 21:28:10.528483 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-05-05 21:27:57.108341 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-05-05 21:28:10.532483 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-05-05 21:28:10.560484 windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-05-05 21:28:10.572484 windmill_api-1.95.0/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-05-05 21:27:57.280342 windmill_api-1.95.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     2644 2023-05-05 21:28:10.596484 windmill_api-1.95.0/windmill_api/models/get_input_history_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-05-05 21:28:10.632484 windmill_api-1.95.0/windmill_api/models/get_input_history_response_200_item_args.py
--rw-r--r--   0        0        0      218 2023-05-05 21:27:56.628336 windmill_api-1.95.0/windmill_api/models/get_input_history_runnable_type.py
--rw-r--r--   0        0        0     1852 2023-05-05 21:28:10.628484 windmill_api-1.95.0/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-05-05 21:27:56.812337 windmill_api-1.95.0/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-05-05 21:28:10.724485 windmill_api-1.95.0/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-05-05 21:28:10.660485 windmill_api-1.95.0/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-05-05 21:28:10.708485 windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-05-05 21:27:56.256332 windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-05-05 21:28:10.732485 windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-05-05 21:28:10.768486 windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-05-05 21:27:56.696336 windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-05-05 21:28:10.756486 windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-05-05 21:28:10.776486 windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-05-05 21:28:10.816486 windmill_api-1.95.0/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-05 21:28:10.796486 windmill_api-1.95.0/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-05-05 21:28:10.832486 windmill_api-1.95.0/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-05-05 21:28:10.844487 windmill_api-1.95.0/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4325 2023-05-05 21:28:10.892487 windmill_api-1.95.0/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-05-05 21:28:10.864487 windmill_api-1.95.0/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-05-05 21:28:10.884487 windmill_api-1.95.0/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     7558 2023-05-05 21:28:10.972488 windmill_api-1.95.0/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-05 21:28:10.908487 windmill_api-1.95.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-05 21:27:57.332343 windmill_api-1.95.0/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-05 21:27:56.792337 windmill_api-1.95.0/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-05 21:28:10.932487 windmill_api-1.95.0/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     7558 2023-05-05 21:28:11.064489 windmill_api-1.95.0/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-05 21:28:10.992488 windmill_api-1.95.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-05 21:27:56.992339 windmill_api-1.95.0/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-05 21:27:56.808338 windmill_api-1.95.0/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-05 21:28:11.016488 windmill_api-1.95.0/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     6383 2023-05-05 21:28:11.168490 windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5608 2023-05-05 21:28:11.136489 windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0      269 2023-05-05 21:27:56.584335 windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
--rw-r--r--   0        0        0      227 2023-05-05 21:27:57.308343 windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
--rw-r--r--   0        0        0     1347 2023-05-05 21:28:11.160490 windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0      264 2023-05-05 21:27:56.380333 windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
--rw-r--r--   0        0        0      222 2023-05-05 21:27:57.292343 windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
--rw-r--r--   0        0        0     1319 2023-05-05 21:28:11.184490 windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-05-05 21:28:11.196490 windmill_api-1.95.0/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-05-05 21:28:11.236491 windmill_api-1.95.0/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-05-05 21:28:11.224491 windmill_api-1.95.0/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-05-05 21:28:11.248491 windmill_api-1.95.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-05-05 21:28:11.268491 windmill_api-1.95.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-05-05 21:27:56.312332 windmill_api-1.95.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-05-05 21:28:11.308491 windmill_api-1.95.0/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-05 21:28:11.288491 windmill_api-1.95.0/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-05-05 21:28:11.324492 windmill_api-1.95.0/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-05-05 21:27:56.704336 windmill_api-1.95.0/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-05-05 21:28:11.336492 windmill_api-1.95.0/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-05-05 21:28:11.364492 windmill_api-1.95.0/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-05-05 21:27:56.420333 windmill_api-1.95.0/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-05-05 21:28:11.372492 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-05-05 21:28:11.468493 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-05-05 21:27:56.772337 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-05-05 21:28:11.400492 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-05-05 21:28:11.428493 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-05-05 21:28:11.452493 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-05-05 21:28:11.548494 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-05-05 21:27:56.264332 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-05-05 21:28:11.496493 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-05-05 21:28:11.532494 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-05-05 21:27:56.448334 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-05 21:28:11.556494 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-05-05 21:27:56.680336 windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-05-05 21:28:11.596494 windmill_api-1.95.0/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-05-05 21:28:11.576494 windmill_api-1.95.0/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-05-05 21:28:11.604494 windmill_api-1.95.0/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-05-05 21:27:56.560335 windmill_api-1.95.0/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     2377 2023-05-05 21:28:11.632495 windmill_api-1.95.0/windmill_api/models/input_.py
--rw-r--r--   0        0        0     1138 2023-05-05 21:28:11.624495 windmill_api-1.95.0/windmill_api/models/input_args.py
--rw-r--r--   0        0        0     1820 2023-05-05 21:28:11.652495 windmill_api-1.95.0/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-05-05 21:27:56.704336 windmill_api-1.95.0/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-05-05 21:28:11.660495 windmill_api-1.95.0/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-05-05 21:27:57.172341 windmill_api-1.95.0/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-05-05 21:28:11.680495 windmill_api-1.95.0/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-05-05 21:28:11.684495 windmill_api-1.95.0/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-05-05 21:27:56.716336 windmill_api-1.95.0/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-05-05 21:28:11.712496 windmill_api-1.95.0/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-05-05 21:27:57.208342 windmill_api-1.95.0/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-05-05 21:28:11.736496 windmill_api-1.95.0/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-05-05 21:27:56.396333 windmill_api-1.95.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-05-05 21:28:11.728496 windmill_api-1.95.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-05-05 21:27:56.860338 windmill_api-1.95.0/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-05-05 21:28:11.776496 windmill_api-1.95.0/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-05-05 21:27:57.280342 windmill_api-1.95.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-05-05 21:27:56.832338 windmill_api-1.95.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-05-05 21:28:11.760496 windmill_api-1.95.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11220 2023-05-05 21:28:11.960498 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-05-05 21:28:11.796496 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-05-05 21:28:11.876497 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-05-05 21:28:11.960498 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-05-05 21:28:11.984498 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-05-05 21:28:11.992498 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-05-05 21:27:56.516334 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-05-05 21:28:12.008499 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-05-05 21:28:12.028499 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-05-05 21:27:56.700336 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-05-05 21:28:12.088499 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-05-05 21:28:12.052499 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-05-05 21:28:12.080500 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-05-05 21:27:56.604335 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-05-05 21:28:12.108500 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-05-05 21:28:12.124500 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-05-05 21:27:56.780337 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-05-05 21:28:12.144500 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-05-05 21:27:57.172341 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-05-05 21:27:56.776337 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-05-05 21:28:12.176500 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-05-05 21:28:12.224501 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-05-05 21:28:12.272501 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-05-05 21:28:12.252501 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-05-05 21:28:12.288502 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-05-05 21:28:12.300502 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-05-05 21:27:56.224331 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-05-05 21:28:12.380503 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-05-05 21:27:56.904338 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-05-05 21:28:12.328502 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-05-05 21:28:12.356502 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-05-05 21:28:12.436503 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-05-05 21:28:12.420503 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-05-05 21:28:12.448503 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-05-05 21:28:12.464503 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-05-05 21:28:12.480504 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-05-05 21:27:56.248331 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-05-05 21:28:12.492504 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-05-05 21:27:56.568335 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-05-05 21:28:12.512504 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-05-05 21:28:12.524504 windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-05-05 21:28:12.540504 windmill_api-1.95.0/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     1863 2023-05-05 21:28:12.552504 windmill_api-1.95.0/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     2074 2023-05-05 21:28:12.568504 windmill_api-1.95.0/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-05 21:28:12.620505 windmill_api-1.95.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-05-05 21:28:12.612505 windmill_api-1.95.0/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-05-05 21:28:12.632505 windmill_api-1.95.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-05-05 21:28:12.652505 windmill_api-1.95.0/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-05-05 21:28:12.668506 windmill_api-1.95.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-05-05 21:28:12.684506 windmill_api-1.95.0/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-05-05 21:28:12.704506 windmill_api-1.95.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-05-05 21:28:12.712506 windmill_api-1.95.0/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-05-05 21:28:12.744506 windmill_api-1.95.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-05-05 21:27:56.956339 windmill_api-1.95.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     2590 2023-05-05 21:28:12.752506 windmill_api-1.95.0/windmill_api/models/list_inputs_response_200_item.py
--rw-r--r--   0        0        0     1250 2023-05-05 21:28:12.764506 windmill_api-1.95.0/windmill_api/models/list_inputs_response_200_item_args.py
--rw-r--r--   0        0        0      213 2023-05-05 21:27:56.808338 windmill_api-1.95.0/windmill_api/models/list_inputs_runnable_type.py
--rw-r--r--   0        0        0     1922 2023-05-05 21:28:12.780507 windmill_api-1.95.0/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-05-05 21:27:56.228331 windmill_api-1.95.0/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-05-05 21:28:12.796507 windmill_api-1.95.0/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    12114 2023-05-05 21:28:12.924508 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-05-05 21:28:12.816507 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-05-05 21:28:12.860507 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-05-05 21:28:13.012509 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-05-05 21:28:12.952508 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-05 21:28:13.036509 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-05 21:27:57.340343 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-05 21:28:13.040509 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-05 21:28:13.072509 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-05-05 21:27:56.916339 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-05-05 21:28:13.124510 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-05-05 21:28:13.096510 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-05-05 21:28:13.124510 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-05-05 21:27:57.152341 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-05-05 21:28:13.152510 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-05-05 21:28:13.160510 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-05-05 21:27:56.656336 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-05-05 21:28:13.184511 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-05-05 21:27:57.352343 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-05-05 21:27:56.804337 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-05-05 21:28:13.200511 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-05-05 21:28:13.264511 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-05-05 21:28:13.240511 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-05-05 21:28:13.268511 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-05 21:28:13.296512 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-05 21:28:13.296512 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-05 21:27:57.012340 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-05 21:28:13.392513 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-05 21:27:56.648336 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-05 21:28:13.324512 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-05 21:28:13.408513 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-05-05 21:28:13.476513 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-05-05 21:28:13.448513 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-05-05 21:28:13.472513 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-05 21:28:13.504514 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-05 21:28:13.504514 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-05 21:27:56.804337 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-05 21:28:13.532514 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-05 21:27:56.532334 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-05 21:28:13.532514 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-05 21:28:13.560514 windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     4884 2023-05-05 21:28:13.596515 windmill_api-1.95.0/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-05 21:28:13.580515 windmill_api-1.95.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-05-05 21:28:13.612515 windmill_api-1.95.0/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4426 2023-05-05 21:28:13.656515 windmill_api-1.95.0/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-05-05 21:28:13.632515 windmill_api-1.95.0/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-05-05 21:28:13.652515 windmill_api-1.95.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     7551 2023-05-05 21:28:13.816517 windmill_api-1.95.0/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-05 21:28:13.672515 windmill_api-1.95.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-05 21:27:57.096341 windmill_api-1.95.0/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-05-05 21:27:57.092341 windmill_api-1.95.0/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-05-05 21:28:13.696516 windmill_api-1.95.0/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-05-05 21:28:13.736516 windmill_api-1.95.0/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-05-05 21:28:13.820517 windmill_api-1.95.0/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-05-05 21:28:13.840517 windmill_api-1.95.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-05-05 21:28:13.856517 windmill_api-1.95.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-05-05 21:27:57.116341 windmill_api-1.95.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4307 2023-05-05 21:28:13.900518 windmill_api-1.95.0/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-05-05 21:28:13.880517 windmill_api-1.95.0/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-05-05 21:28:13.944518 windmill_api-1.95.0/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-05 21:28:13.920518 windmill_api-1.95.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-05-05 21:28:13.956518 windmill_api-1.95.0/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-05-05 21:28:13.972518 windmill_api-1.95.0/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-05-05 21:28:13.988518 windmill_api-1.95.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-05-05 21:28:14.004519 windmill_api-1.95.0/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-05-05 21:28:14.032519 windmill_api-1.95.0/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-05-05 21:27:56.896338 windmill_api-1.95.0/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-05-05 21:28:14.024519 windmill_api-1.95.0/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-05-05 21:28:14.088519 windmill_api-1.95.0/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-05-05 21:28:14.052519 windmill_api-1.95.0/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-05-05 21:28:14.112520 windmill_api-1.95.0/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-05-05 21:28:14.104519 windmill_api-1.95.0/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-05-05 21:28:14.132520 windmill_api-1.95.0/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-05-05 21:28:14.136520 windmill_api-1.95.0/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-05-05 21:28:14.208521 windmill_api-1.95.0/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-05-05 21:28:14.176520 windmill_api-1.95.0/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-05-05 21:28:14.300521 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-05-05 21:27:56.920339 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-05-05 21:28:14.232521 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-05-05 21:28:14.256521 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-05-05 21:28:14.284521 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-05-05 21:28:14.320522 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-05-05 21:27:56.360333 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-05 21:28:14.324522 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-05-05 21:28:14.356522 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-05-05 21:27:56.396333 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-05-05 21:28:14.348522 windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-05-05 21:27:56.360333 windmill_api-1.95.0/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2662 2023-05-05 21:28:14.392522 windmill_api-1.95.0/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-05-05 21:28:14.376522 windmill_api-1.95.0/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     4866 2023-05-05 21:28:14.444523 windmill_api-1.95.0/windmill_api/models/new_script.py
--rw-r--r--   0        0        0      238 2023-05-05 21:27:56.960339 windmill_api-1.95.0/windmill_api/models/new_script_kind.py
--rw-r--r--   0        0        0      196 2023-05-05 21:27:57.120341 windmill_api-1.95.0/windmill_api/models/new_script_language.py
--rw-r--r--   0        0        0     1171 2023-05-05 21:28:14.412523 windmill_api-1.95.0/windmill_api/models/new_script_schema.py
--rw-r--r--   0        0        0     5879 2023-05-05 21:28:14.496523 windmill_api-1.95.0/windmill_api/models/new_script_with_draft.py
--rw-r--r--   0        0        0     5192 2023-05-05 21:28:14.512524 windmill_api-1.95.0/windmill_api/models/new_script_with_draft_draft.py
--rw-r--r--   0        0        0      252 2023-05-05 21:27:56.576335 windmill_api-1.95.0/windmill_api/models/new_script_with_draft_draft_kind.py
--rw-r--r--   0        0        0      210 2023-05-05 21:27:56.648336 windmill_api-1.95.0/windmill_api/models/new_script_with_draft_draft_language.py
--rw-r--r--   0        0        0     1250 2023-05-05 21:28:14.520524 windmill_api-1.95.0/windmill_api/models/new_script_with_draft_draft_schema.py
--rw-r--r--   0        0        0      247 2023-05-05 21:27:56.284332 windmill_api-1.95.0/windmill_api/models/new_script_with_draft_kind.py
--rw-r--r--   0        0        0      205 2023-05-05 21:27:56.644336 windmill_api-1.95.0/windmill_api/models/new_script_with_draft_language.py
--rw-r--r--   0        0        0     1222 2023-05-05 21:28:14.536524 windmill_api-1.95.0/windmill_api/models/new_script_with_draft_schema.py
--rw-r--r--   0        0        0     2108 2023-05-05 21:28:14.552524 windmill_api-1.95.0/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     2473 2023-05-05 21:28:14.624525 windmill_api-1.95.0/windmill_api/models/new_token_impersonate.py
--rw-r--r--   0        0        0     1710 2023-05-05 21:28:14.580524 windmill_api-1.95.0/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-05-05 21:28:14.620525 windmill_api-1.95.0/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-05-05 21:28:14.640525 windmill_api-1.95.0/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-05-05 21:28:14.664525 windmill_api-1.95.0/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-05-05 21:28:14.792526 windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-05-05 21:28:14.704526 windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-05-05 21:28:14.732526 windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-05-05 21:28:14.764526 windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-05-05 21:28:14.792526 windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-05-05 21:27:56.548335 windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-05-05 21:28:14.820527 windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-05-05 21:27:57.188341 windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-05-05 21:28:14.824527 windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-05-05 21:28:14.848527 windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-05-05 21:28:14.904528 windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-05-05 21:28:14.884527 windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-05-05 21:28:14.912527 windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-05-05 21:28:14.936528 windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-05-05 21:28:14.940528 windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-05-05 21:27:56.984339 windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-05-05 21:28:14.964528 windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-05-05 21:27:56.380333 windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-05-05 21:28:14.968528 windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-05-05 21:28:14.992528 windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-05-05 21:28:15.004528 windmill_api-1.95.0/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-05-05 21:28:15.008528 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-05-05 21:28:15.044529 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-05-05 21:28:15.180530 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-05-05 21:28:15.136530 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-05-05 21:28:15.164530 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-05-05 21:28:15.196530 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-05-05 21:28:15.208530 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-05-05 21:27:56.472334 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-05-05 21:28:15.220531 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-05-05 21:27:56.436334 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-05-05 21:28:15.236531 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-05-05 21:28:15.252531 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-05-05 21:28:15.312531 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-05-05 21:28:15.288531 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-05-05 21:28:15.316532 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-05-05 21:28:15.344532 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-05-05 21:28:15.344532 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-05 21:27:56.864338 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-05-05 21:28:15.368532 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-05 21:27:57.296343 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-05-05 21:28:15.372532 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-05-05 21:28:15.396532 windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-05-05 21:28:15.404532 windmill_api-1.95.0/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-05-05 21:28:15.432533 windmill_api-1.95.0/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-05-05 21:28:15.432533 windmill_api-1.95.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-05-05 21:27:56.508334 windmill_api-1.95.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-05-05 21:28:15.508533 windmill_api-1.95.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-05-05 21:27:56.356333 windmill_api-1.95.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-05-05 21:27:56.560335 windmill_api-1.95.0/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-05-05 21:28:15.468533 windmill_api-1.95.0/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-05-05 21:28:15.504533 windmill_api-1.95.0/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-05-05 21:28:15.612534 windmill_api-1.95.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-05-05 21:27:57.216342 windmill_api-1.95.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-05-05 21:28:15.536534 windmill_api-1.95.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-05-05 21:27:56.816337 windmill_api-1.95.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-05-05 21:27:56.844338 windmill_api-1.95.0/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-05-05 21:28:15.584534 windmill_api-1.95.0/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-05-05 21:27:57.312343 windmill_api-1.95.0/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-05-05 21:28:15.608534 windmill_api-1.95.0/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-05-05 21:28:15.628534 windmill_api-1.95.0/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2359 2023-05-05 21:28:15.652535 windmill_api-1.95.0/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-05-05 21:28:15.648535 windmill_api-1.95.0/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-05-05 21:27:57.144341 windmill_api-1.95.0/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1642 2023-05-05 21:28:15.676535 windmill_api-1.95.0/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-05-05 21:28:15.692535 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-05-05 21:28:15.736536 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-05-05 21:27:56.364333 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-05-05 21:28:15.716535 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-05-05 21:28:15.740536 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-05-05 21:28:15.760536 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-05-05 21:28:15.776536 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-05-05 21:27:57.064340 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-05-05 21:28:15.788536 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-05-05 21:28:15.816536 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-05-05 21:27:56.244331 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-05-05 21:28:15.812536 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-05-05 21:27:57.240342 windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11580 2023-05-05 21:28:16.016538 windmill_api-1.95.0/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-05-05 21:28:15.832537 windmill_api-1.95.0/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-05-05 21:28:15.876537 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-05-05 21:28:15.956538 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-05-05 21:28:15.980538 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-05-05 21:28:16.100539 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-05-05 21:27:56.844338 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-05-05 21:28:16.044539 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-05-05 21:28:16.076539 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-05-05 21:27:56.864338 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-05-05 21:28:16.156540 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-05-05 21:28:16.128539 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-05-05 21:28:16.156540 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-05-05 21:27:56.448334 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-05-05 21:28:16.180540 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-05-05 21:28:16.192540 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-05-05 21:27:56.232331 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-05-05 21:28:16.212540 windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-05-05 21:27:57.124341 windmill_api-1.95.0/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-05-05 21:27:56.584335 windmill_api-1.95.0/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-05-05 21:28:16.236540 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-05-05 21:28:16.292541 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-05-05 21:28:16.336542 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-05-05 21:28:16.320541 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-05-05 21:28:16.352542 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-05-05 21:28:16.364542 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-05 21:27:56.972339 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-05-05 21:28:16.380542 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-05 21:27:56.904338 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-05-05 21:28:16.392542 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-05-05 21:28:16.408542 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-05-05 21:28:16.472543 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-05-05 21:28:16.444543 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-05-05 21:28:16.472543 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-05-05 21:28:16.504543 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-05-05 21:28:16.500543 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-05 21:27:57.116341 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-05-05 21:28:16.528543 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-05 21:27:56.792337 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-05-05 21:28:16.532543 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-05-05 21:28:16.556544 windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     3028 2023-05-05 21:28:16.572544 windmill_api-1.95.0/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-05-05 21:28:16.680545 windmill_api-1.95.0/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-05-05 21:28:16.600544 windmill_api-1.95.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-05-05 21:27:56.812337 windmill_api-1.95.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-05-05 21:28:16.628544 windmill_api-1.95.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-05-05 21:27:56.752337 windmill_api-1.95.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-05-05 21:27:57.232342 windmill_api-1.95.0/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-05-05 21:27:56.256332 windmill_api-1.95.0/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-05-05 21:28:16.656545 windmill_api-1.95.0/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-05-05 21:28:16.676545 windmill_api-1.95.0/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      304 2023-05-05 21:27:56.624335 windmill_api-1.95.0/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-05-05 21:28:16.700545 windmill_api-1.95.0/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-05-05 21:28:16.704545 windmill_api-1.95.0/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-05-05 21:28:16.748546 windmill_api-1.95.0/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-05-05 21:28:16.724545 windmill_api-1.95.0/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-05-05 21:28:16.756546 windmill_api-1.95.0/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-05-05 21:28:16.768546 windmill_api-1.95.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-05 21:28:16.824546 windmill_api-1.95.0/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-05-05 21:28:16.808546 windmill_api-1.95.0/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-05-05 21:28:16.836546 windmill_api-1.95.0/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-05-05 21:28:16.856546 windmill_api-1.95.0/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-05-05 21:28:16.856546 windmill_api-1.95.0/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-05-05 21:28:16.888547 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-05-05 21:28:16.876547 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-05-05 21:28:16.916547 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-05-05 21:28:16.968548 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-05-05 21:28:16.952547 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-05-05 21:28:16.980548 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-05-05 21:28:17.000548 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-05-05 21:28:17.008548 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-05 21:27:56.404333 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-05-05 21:28:17.028548 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-05 21:27:56.348333 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-05-05 21:28:17.036548 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-05-05 21:28:17.056548 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-05-05 21:28:17.116549 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-05-05 21:28:17.092549 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-05-05 21:28:17.120549 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-05-05 21:28:17.212550 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-05-05 21:28:17.148549 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-05-05 21:27:57.176341 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-05-05 21:28:17.176550 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-05-05 21:27:57.004340 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-05-05 21:28:17.204550 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-05-05 21:28:17.328551 windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-05-05 21:28:17.228550 windmill_api-1.95.0/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-05-05 21:28:17.248551 windmill_api-1.95.0/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2634 2023-05-05 21:28:17.284551 windmill_api-1.95.0/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-05-05 21:28:17.308551 windmill_api-1.95.0/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-05-05 21:27:57.092341 windmill_api-1.95.0/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-05-05 21:28:17.328551 windmill_api-1.95.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-05-05 21:28:17.344551 windmill_api-1.95.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0      203 2023-05-05 21:27:57.048340 windmill_api-1.95.0/windmill_api/models/runnable_type.py
--rw-r--r--   0        0        0     4086 2023-05-05 21:28:17.388552 windmill_api-1.95.0/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-05-05 21:28:17.364552 windmill_api-1.95.0/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-05-05 21:28:17.384552 windmill_api-1.95.0/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     7003 2023-05-05 21:28:17.476553 windmill_api-1.95.0/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-05-05 21:28:17.408552 windmill_api-1.95.0/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-05-05 21:28:17.428552 windmill_api-1.95.0/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-05-05 21:27:56.972339 windmill_api-1.95.0/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-05-05 21:27:57.184342 windmill_api-1.95.0/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-05-05 21:28:17.448552 windmill_api-1.95.0/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-05-05 21:28:17.472553 windmill_api-1.95.0/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-05-05 21:28:17.492553 windmill_api-1.95.0/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-05-05 21:28:17.504553 windmill_api-1.95.0/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-05-05 21:28:17.516553 windmill_api-1.95.0/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-05-05 21:28:17.536553 windmill_api-1.95.0/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      185 2023-05-05 21:27:57.108341 windmill_api-1.95.0/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-05-05 21:28:17.548553 windmill_api-1.95.0/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-05-05 21:27:56.880338 windmill_api-1.95.0/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-05-05 21:28:17.576554 windmill_api-1.95.0/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-05-05 21:28:17.588554 windmill_api-1.95.0/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-05-05 21:28:17.608554 windmill_api-1.95.0/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      187 2023-05-05 21:27:57.064340 windmill_api-1.95.0/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-05-05 21:28:17.628554 windmill_api-1.95.0/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-05 21:28:17.652554 windmill_api-1.95.0/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-05 21:27:56.704336 windmill_api-1.95.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-05 21:28:17.656554 windmill_api-1.95.0/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-05 21:28:17.672555 windmill_api-1.95.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-05-05 21:28:17.760555 windmill_api-1.95.0/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-05-05 21:28:17.688555 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-05-05 21:28:17.732555 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-05-05 21:28:17.904557 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-05-05 21:28:17.796556 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-05-05 21:28:17.824556 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-05-05 21:28:17.856556 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-05-05 21:28:17.884557 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-05-05 21:27:57.076340 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-05-05 21:28:17.916557 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-05-05 21:27:57.224342 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-05-05 21:28:17.932557 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-05-05 21:28:17.940557 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-05-05 21:28:18.012558 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-05-05 21:28:17.980558 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-05-05 21:28:18.008558 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-05-05 21:28:18.040558 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-05-05 21:28:18.040558 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-05-05 21:27:56.788337 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-05-05 21:28:18.064558 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-05-05 21:27:56.976339 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-05-05 21:28:18.068559 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-05-05 21:28:18.092559 windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-05-05 21:28:18.100559 windmill_api-1.95.0/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-05-05 21:28:18.116559 windmill_api-1.95.0/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     1670 2023-05-05 21:28:18.128559 windmill_api-1.95.0/windmill_api/models/update_input.py
--rw-r--r--   0        0        0     1716 2023-05-05 21:28:18.144559 windmill_api-1.95.0/windmill_api/models/update_input_json_body.py
--rw-r--r--   0        0        0     2036 2023-05-05 21:28:18.160559 windmill_api-1.95.0/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-05-05 21:28:18.172559 windmill_api-1.95.0/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-05-05 21:28:18.184560 windmill_api-1.95.0/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1953 2023-05-05 21:28:18.200560 windmill_api-1.95.0/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-05 21:28:18.204560 windmill_api-1.95.0/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-05-05 21:28:18.228560 windmill_api-1.95.0/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-05-05 21:28:18.236560 windmill_api-1.95.0/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-05-05 21:28:18.252560 windmill_api-1.95.0/windmill_api/models/usage.py
--rw-r--r--   0        0        0     4071 2023-05-05 21:28:18.356561 windmill_api-1.95.0/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-05-05 21:28:18.276560 windmill_api-1.95.0/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-05-05 21:28:18.304561 windmill_api-1.95.0/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-05-05 21:28:18.332561 windmill_api-1.95.0/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     4222 2023-05-05 21:28:18.504563 windmill_api-1.95.0/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-05-05 21:28:18.380561 windmill_api-1.95.0/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     4211 2023-05-05 21:28:18.440562 windmill_api-1.95.0/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-05-05 21:28:18.464562 windmill_api-1.95.0/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-05-05 21:28:18.500563 windmill_api-1.95.0/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-05-05 21:28:18.532563 windmill_api-1.95.0/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-05-05 21:28:18.536563 windmill_api-1.95.0/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-05-05 21:27:47.100202 windmill_api-1.95.0/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-05-05 21:28:18.548563 windmill_api-1.95.0/windmill_api/types.py
--rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 windmill_api-1.95.0/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.95.0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-06 10:11:34.669474 windmill_api-1.95.1/LICENSE
+-rw-r--r--   0        0        0     2952 2023-05-06 10:11:34.673474 windmill_api-1.95.1/README.md
+-rw-r--r--   0        0        0      717 2023-05-06 10:11:34.673474 windmill_api-1.95.1/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-06 10:11:01.929416 windmill_api-1.95.1/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-06 10:11:02.413417 windmill_api-1.95.1/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.521417 windmill_api-1.95.1/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-05-06 10:11:13.217443 windmill_api-1.95.1/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-05-06 10:11:13.229443 windmill_api-1.95.1/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-05-06 10:11:13.265443 windmill_api-1.95.1/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-05-06 10:11:13.269443 windmill_api-1.95.1/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-05-06 10:11:13.309443 windmill_api-1.95.1/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3187 2023-05-06 10:11:13.313443 windmill_api-1.95.1/windmill_api/api/app/get_app_by_path_with_draft.py
+-rw-r--r--   0        0        0     3031 2023-05-06 10:11:13.349443 windmill_api-1.95.1/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-05-06 10:11:13.361443 windmill_api-1.95.1/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-05-06 10:11:13.409443 windmill_api-1.95.1/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-05-06 10:11:13.393443 windmill_api-1.95.1/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-05-06 10:11:13.489444 windmill_api-1.95.1/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-05-06 10:11:13.441444 windmill_api-1.95.1/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-05-06 10:11:13.473444 windmill_api-1.95.1/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.453417 windmill_api-1.95.1/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-05-06 10:11:13.517444 windmill_api-1.95.1/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-05-06 10:11:13.605444 windmill_api-1.95.1/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.585417 windmill_api-1.95.1/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-05-06 10:11:13.545444 windmill_api-1.95.1/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-05-06 10:11:13.573444 windmill_api-1.95.1/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-05-06 10:11:13.601444 windmill_api-1.95.1/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.541417 windmill_api-1.95.1/windmill_api/api/draft/__init__.py
+-rw-r--r--   0        0        0     2019 2023-05-06 10:11:13.633444 windmill_api-1.95.1/windmill_api/api/draft/create_draft.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.589418 windmill_api-1.95.1/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-05-06 10:11:13.641444 windmill_api-1.95.1/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-05-06 10:11:13.661444 windmill_api-1.95.1/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.509417 windmill_api-1.95.1/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-06 10:11:13.673444 windmill_api-1.95.1/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-05-06 10:11:13.693444 windmill_api-1.95.1/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-05-06 10:11:13.705444 windmill_api-1.95.1/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-05-06 10:11:13.745444 windmill_api-1.95.1/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-05-06 10:11:13.765444 windmill_api-1.95.1/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     3205 2023-05-06 10:11:13.785444 windmill_api-1.95.1/windmill_api/api/flow/get_flow_by_path_with_draft.py
+-rw-r--r--   0        0        0     4827 2023-05-06 10:11:13.829445 windmill_api-1.95.1/windmill_api/api/flow/get_flow_input_history_by_path.py
+-rw-r--r--   0        0        0     2667 2023-05-06 10:11:13.825444 windmill_api-1.95.1/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-05-06 10:11:13.853444 windmill_api-1.95.1/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-05-06 10:11:13.933445 windmill_api-1.95.1/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-05-06 10:11:13.885444 windmill_api-1.95.1/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-05-06 10:11:13.917445 windmill_api-1.95.1/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.577417 windmill_api-1.95.1/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-06 10:11:13.949445 windmill_api-1.95.1/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-05-06 10:11:13.965445 windmill_api-1.95.1/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-05-06 10:11:13.977445 windmill_api-1.95.1/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-05-06 10:11:14.009445 windmill_api-1.95.1/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-05-06 10:11:14.017445 windmill_api-1.95.1/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-05-06 10:11:14.061445 windmill_api-1.95.1/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-05-06 10:11:14.093445 windmill_api-1.95.1/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-05-06 10:11:14.097445 windmill_api-1.95.1/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-05-06 10:11:14.125445 windmill_api-1.95.1/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.585417 windmill_api-1.95.1/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-05-06 10:11:14.149445 windmill_api-1.95.1/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-05-06 10:11:14.173445 windmill_api-1.95.1/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-05-06 10:11:14.181445 windmill_api-1.95.1/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.573417 windmill_api-1.95.1/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-05-06 10:11:14.209445 windmill_api-1.95.1/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-05-06 10:11:14.209445 windmill_api-1.95.1/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-05-06 10:11:14.237445 windmill_api-1.95.1/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-05-06 10:11:14.253445 windmill_api-1.95.1/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-05-06 10:11:14.289445 windmill_api-1.95.1/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-05-06 10:11:14.317446 windmill_api-1.95.1/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-05-06 10:11:14.317446 windmill_api-1.95.1/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-05-06 10:11:14.349446 windmill_api-1.95.1/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.589418 windmill_api-1.95.1/windmill_api/api/input_/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-06 10:11:14.365446 windmill_api-1.95.1/windmill_api/api/input_/create_input.py
+-rw-r--r--   0        0        0     1811 2023-05-06 10:11:14.377446 windmill_api-1.95.1/windmill_api/api/input_/delete_input.py
+-rw-r--r--   0        0        0     6187 2023-05-06 10:11:14.461446 windmill_api-1.95.1/windmill_api/api/input_/get_input_history.py
+-rw-r--r--   0        0        0     6010 2023-05-06 10:11:14.449446 windmill_api-1.95.1/windmill_api/api/input_/list_inputs.py
+-rw-r--r--   0        0        0     2025 2023-05-06 10:11:14.497446 windmill_api-1.95.1/windmill_api/api/input_/update_input.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.545417 windmill_api-1.95.1/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-05-06 10:11:14.493446 windmill_api-1.95.1/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-05-06 10:11:14.537446 windmill_api-1.95.1/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-06 10:11:14.541446 windmill_api-1.95.1/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-05-06 10:11:14.577446 windmill_api-1.95.1/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-05-06 10:11:14.581446 windmill_api-1.95.1/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-05-06 10:11:14.609446 windmill_api-1.95.1/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-05-06 10:11:14.621446 windmill_api-1.95.1/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-05-06 10:11:14.637446 windmill_api-1.95.1/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-05-06 10:11:14.661446 windmill_api-1.95.1/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-05-06 10:11:14.697446 windmill_api-1.95.1/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-05-06 10:11:14.721446 windmill_api-1.95.1/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-05-06 10:11:14.757446 windmill_api-1.95.1/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    13065 2023-05-06 10:11:14.889447 windmill_api-1.95.1/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    12292 2023-05-06 10:11:14.917447 windmill_api-1.95.1/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12830 2023-05-06 10:11:15.045447 windmill_api-1.95.1/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-05-06 10:11:14.949447 windmill_api-1.95.1/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-05-06 10:11:14.981447 windmill_api-1.95.1/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-05-06 10:11:15.029447 windmill_api-1.95.1/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-06 10:11:15.073447 windmill_api-1.95.1/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-05-06 10:11:15.101447 windmill_api-1.95.1/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-05-06 10:11:15.117447 windmill_api-1.95.1/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-05-06 10:11:15.161447 windmill_api-1.95.1/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-05-06 10:11:15.193447 windmill_api-1.95.1/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-05-06 10:11:15.201447 windmill_api-1.95.1/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-05-06 10:11:15.237448 windmill_api-1.95.1/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-05-06 10:11:15.273448 windmill_api-1.95.1/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-05-06 10:11:15.289448 windmill_api-1.95.1/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.485417 windmill_api-1.95.1/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-06 10:11:15.313448 windmill_api-1.95.1/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-05-06 10:11:15.321448 windmill_api-1.95.1/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-05-06 10:11:15.345448 windmill_api-1.95.1/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-05-06 10:11:15.353448 windmill_api-1.95.1/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-05-06 10:11:15.369448 windmill_api-1.95.1/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-05-06 10:11:15.385448 windmill_api-1.95.1/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-05-06 10:11:15.405448 windmill_api-1.95.1/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-05-06 10:11:15.421448 windmill_api-1.95.1/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.489417 windmill_api-1.95.1/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-06 10:11:15.437448 windmill_api-1.95.1/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-05-06 10:11:15.453448 windmill_api-1.95.1/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-05-06 10:11:15.465448 windmill_api-1.95.1/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-05-06 10:11:15.485448 windmill_api-1.95.1/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-05-06 10:11:15.505448 windmill_api-1.95.1/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-05-06 10:11:15.529448 windmill_api-1.95.1/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-05-06 10:11:15.545448 windmill_api-1.95.1/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-05-06 10:11:15.585448 windmill_api-1.95.1/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-05-06 10:11:15.589448 windmill_api-1.95.1/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-05-06 10:11:15.661449 windmill_api-1.95.1/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-05-06 10:11:15.629449 windmill_api-1.95.1/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-05-06 10:11:15.669448 windmill_api-1.95.1/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-05-06 10:11:15.693449 windmill_api-1.95.1/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-05-06 10:11:15.697449 windmill_api-1.95.1/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-05-06 10:11:15.729449 windmill_api-1.95.1/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.569417 windmill_api-1.95.1/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-06 10:11:15.729449 windmill_api-1.95.1/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-05-06 10:11:15.757449 windmill_api-1.95.1/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-05-06 10:11:15.769449 windmill_api-1.95.1/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-05-06 10:11:15.801449 windmill_api-1.95.1/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-05-06 10:11:15.829449 windmill_api-1.95.1/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-05-06 10:11:15.849449 windmill_api-1.95.1/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-05-06 10:11:15.861449 windmill_api-1.95.1/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-05-06 10:11:15.881449 windmill_api-1.95.1/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.497417 windmill_api-1.95.1/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-06 10:11:15.901449 windmill_api-1.95.1/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-05-06 10:11:15.913449 windmill_api-1.95.1/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-06 10:11:15.949449 windmill_api-1.95.1/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-05-06 10:11:15.957449 windmill_api-1.95.1/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-05-06 10:11:15.989449 windmill_api-1.95.1/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-05-06 10:11:16.001449 windmill_api-1.95.1/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-06 10:11:16.029449 windmill_api-1.95.1/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-05-06 10:11:16.045449 windmill_api-1.95.1/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-05-06 10:11:16.069449 windmill_api-1.95.1/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-05-06 10:11:16.073449 windmill_api-1.95.1/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-05-06 10:11:16.109449 windmill_api-1.95.1/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-05-06 10:11:16.117449 windmill_api-1.95.1/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3241 2023-05-06 10:11:16.149449 windmill_api-1.95.1/windmill_api/api/script/get_script_by_path_with_draft.py
+-rw-r--r--   0        0        0     3276 2023-05-06 10:11:16.157450 windmill_api-1.95.1/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-05-06 10:11:16.189450 windmill_api-1.95.1/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-05-06 10:11:16.193450 windmill_api-1.95.1/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-05-06 10:11:16.213450 windmill_api-1.95.1/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-05-06 10:11:16.349450 windmill_api-1.95.1/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-05-06 10:11:16.269450 windmill_api-1.95.1/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-05-06 10:11:16.297450 windmill_api-1.95.1/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-05-06 10:11:16.325450 windmill_api-1.95.1/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-05-06 10:11:16.357450 windmill_api-1.95.1/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.425417 windmill_api-1.95.1/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-06 10:11:16.377450 windmill_api-1.95.1/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-05-06 10:11:16.381450 windmill_api-1.95.1/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.457417 windmill_api-1.95.1/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-05-06 10:11:16.405450 windmill_api-1.95.1/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-05-06 10:11:16.413450 windmill_api-1.95.1/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-05-06 10:11:16.433450 windmill_api-1.95.1/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-05-06 10:11:16.445450 windmill_api-1.95.1/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-05-06 10:11:16.461450 windmill_api-1.95.1/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-05-06 10:11:16.473450 windmill_api-1.95.1/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-05-06 10:11:16.485450 windmill_api-1.95.1/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-05-06 10:11:16.505450 windmill_api-1.95.1/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-05-06 10:11:16.509450 windmill_api-1.95.1/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-05-06 10:11:16.529450 windmill_api-1.95.1/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-05-06 10:11:16.537450 windmill_api-1.95.1/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-05-06 10:11:16.561450 windmill_api-1.95.1/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-05-06 10:11:16.581451 windmill_api-1.95.1/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-05-06 10:11:16.613451 windmill_api-1.95.1/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-05-06 10:11:16.609450 windmill_api-1.95.1/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-05-06 10:11:16.649451 windmill_api-1.95.1/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-05-06 10:11:16.649451 windmill_api-1.95.1/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-05-06 10:11:16.709451 windmill_api-1.95.1/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-05-06 10:11:16.705451 windmill_api-1.95.1/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-05-06 10:11:16.745451 windmill_api-1.95.1/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-05-06 10:11:16.737451 windmill_api-1.95.1/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-05-06 10:11:16.769451 windmill_api-1.95.1/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-05-06 10:11:16.769451 windmill_api-1.95.1/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-05-06 10:11:16.797451 windmill_api-1.95.1/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-05-06 10:11:16.801451 windmill_api-1.95.1/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-05-06 10:11:16.837451 windmill_api-1.95.1/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-05-06 10:11:16.841451 windmill_api-1.95.1/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.477417 windmill_api-1.95.1/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-05-06 10:11:16.881451 windmill_api-1.95.1/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-05-06 10:11:16.869451 windmill_api-1.95.1/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-05-06 10:11:16.913451 windmill_api-1.95.1/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-05-06 10:11:16.933451 windmill_api-1.95.1/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-05-06 10:11:16.969451 windmill_api-1.95.1/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-05-06 10:11:16.977451 windmill_api-1.95.1/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-05-06 10:11:17.009451 windmill_api-1.95.1/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.545417 windmill_api-1.95.1/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     2448 2023-05-06 10:11:17.013451 windmill_api-1.95.1/windmill_api/api/worker/get_custom_tags.py
+-rw-r--r--   0        0        0     3896 2023-05-06 10:11:17.065451 windmill_api-1.95.1/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:11:02.469417 windmill_api-1.95.1/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-06 10:11:17.061452 windmill_api-1.95.1/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-05-06 10:11:17.093452 windmill_api-1.95.1/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-05-06 10:11:17.093452 windmill_api-1.95.1/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-05-06 10:11:17.125452 windmill_api-1.95.1/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-05-06 10:11:17.117452 windmill_api-1.95.1/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-05-06 10:11:17.149452 windmill_api-1.95.1/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-05-06 10:11:17.157452 windmill_api-1.95.1/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-05-06 10:11:17.177452 windmill_api-1.95.1/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-05-06 10:11:17.185452 windmill_api-1.95.1/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-05-06 10:11:17.205452 windmill_api-1.95.1/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-05-06 10:11:17.225452 windmill_api-1.95.1/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-05-06 10:11:17.241452 windmill_api-1.95.1/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-05-06 10:11:17.253452 windmill_api-1.95.1/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-05-06 10:11:17.277452 windmill_api-1.95.1/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-05-06 10:11:17.297452 windmill_api-1.95.1/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-05-06 10:11:17.325452 windmill_api-1.95.1/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-05-06 10:11:17.337452 windmill_api-1.95.1/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-05-06 10:11:17.381452 windmill_api-1.95.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-05-06 10:11:17.365452 windmill_api-1.95.1/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-05-06 10:11:17.409452 windmill_api-1.95.1/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-05-06 10:11:34.665474 windmill_api-1.95.1/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-06 10:11:17.433452 windmill_api-1.95.1/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-05-06 10:11:17.461452 windmill_api-1.95.1/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      301 2023-05-06 10:11:11.853440 windmill_api-1.95.1/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-05-06 10:11:17.493452 windmill_api-1.95.1/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-05-06 10:11:17.525452 windmill_api-1.95.1/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-05-06 10:11:17.525452 windmill_api-1.95.1/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-05-06 10:11:17.577453 windmill_api-1.95.1/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-05-06 10:11:12.337441 windmill_api-1.95.1/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-05-06 10:11:17.549453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-05-06 10:11:17.601453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-05-06 10:11:12.381441 windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-05-06 10:11:17.625453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-05-06 10:11:17.621453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4638 2023-05-06 10:11:17.685453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft.py
+-rw-r--r--   0        0        0      220 2023-05-06 10:11:12.397441 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
+-rw-r--r--   0        0        0     1284 2023-05-06 10:11:17.649453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
+-rw-r--r--   0        0        0     3828 2023-05-06 10:11:17.697453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy.py
+-rw-r--r--   0        0        0      226 2023-05-06 10:11:11.957440 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
+-rw-r--r--   0        0        0     2020 2023-05-06 10:11:17.713453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
+-rw-r--r--   0        0        0     1417 2023-05-06 10:11:17.717453 windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1569 2023-05-06 10:11:17.749453 windmill_api-1.95.1/windmill_api/models/archive_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     7662 2023-05-06 10:11:17.813453 windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-05-06 10:11:17.773453 windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-05-06 10:11:12.605442 windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-05-06 10:11:12.305441 windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-05-06 10:11:17.797453 windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-05-06 10:11:17.869453 windmill_api-1.95.1/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-05-06 10:11:12.373441 windmill_api-1.95.1/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-05-06 10:11:12.265441 windmill_api-1.95.1/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-05-06 10:11:17.837453 windmill_api-1.95.1/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-05-06 10:11:17.885453 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-06 10:11:17.933453 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-06 10:11:12.281441 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-06 10:11:17.909453 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-06 10:11:17.937453 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-06 10:11:17.961454 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-06 10:11:17.977454 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-06 10:11:12.437441 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-06 10:11:17.993454 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-06 10:11:18.033454 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-06 10:11:12.381441 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-06 10:11:18.017454 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-06 10:11:11.705440 windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-05-06 10:11:18.061454 windmill_api-1.95.1/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-05-06 10:11:18.069454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-06 10:11:18.145454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-06 10:11:18.109454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-06 10:11:18.141454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-06 10:11:18.173454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-06 10:11:18.181454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-06 10:11:12.353441 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-06 10:11:18.205454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-06 10:11:11.969440 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-06 10:11:18.229454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-06 10:11:18.233454 windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-06 10:11:11.897440 windmill_api-1.95.1/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-05-06 10:11:18.273454 windmill_api-1.95.1/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-05-06 10:11:18.269454 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-06 10:11:18.353454 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-06 10:11:18.317454 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-06 10:11:18.345454 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-06 10:11:18.381455 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-06 10:11:18.397455 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-06 10:11:12.273441 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-06 10:11:18.413455 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-06 10:11:11.837440 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-06 10:11:18.425454 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-06 10:11:18.445455 windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-06 10:11:18.509455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-05-06 10:11:18.489455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-06 10:11:18.517455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-06 10:11:18.545455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-06 10:11:18.553455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-06 10:11:11.965440 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-06 10:11:18.577455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-06 10:11:12.521442 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-06 10:11:18.585455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-06 10:11:18.605455 windmill_api-1.95.1/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-06 10:11:12.361441 windmill_api-1.95.1/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-05-06 10:11:18.633455 windmill_api-1.95.1/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-06 10:11:18.625455 windmill_api-1.95.1/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10508 2023-05-06 10:11:18.793455 windmill_api-1.95.1/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-05-06 10:11:18.653455 windmill_api-1.95.1/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-05-06 10:11:18.697455 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-05-06 10:11:18.785455 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-05-06 10:11:18.813455 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-05-06 10:11:18.833455 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-05-06 10:11:12.533442 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-05-06 10:11:18.841456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-05-06 10:11:18.873456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-05-06 10:11:11.821440 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-05-06 10:11:18.921456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-05-06 10:11:18.901455 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-05-06 10:11:18.937456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-05-06 10:11:11.593439 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-05-06 10:11:18.949456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-05-06 10:11:18.973456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-05-06 10:11:12.605442 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-05-06 10:11:18.985456 windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-05-06 10:11:12.045441 windmill_api-1.95.1/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-05-06 10:11:11.581440 windmill_api-1.95.1/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-05-06 10:11:19.025456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-05-06 10:11:19.089456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-05-06 10:11:19.069456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-06 10:11:19.101456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-06 10:11:19.121456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-06 10:11:19.133456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-06 10:11:12.133441 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-06 10:11:19.149456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-06 10:11:12.129441 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-06 10:11:19.189456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-06 10:11:19.177456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-05-06 10:11:19.261456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-05-06 10:11:19.229456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-05-06 10:11:19.261456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-05-06 10:11:19.293456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-05-06 10:11:19.293456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-05-06 10:11:11.937440 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-05-06 10:11:19.321457 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-05-06 10:11:11.973440 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-05-06 10:11:19.325456 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-05-06 10:11:19.349457 windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-05-06 10:11:19.357457 windmill_api-1.95.1/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-05-06 10:11:19.389457 windmill_api-1.95.1/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-05-06 10:11:19.405457 windmill_api-1.95.1/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-05-06 10:11:19.417457 windmill_api-1.95.1/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-05-06 10:11:19.437457 windmill_api-1.95.1/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2367 2023-05-06 10:11:19.457457 windmill_api-1.95.1/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-06 10:11:19.485457 windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-06 10:11:12.609442 windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-06 10:11:19.485457 windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-06 10:11:19.509457 windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1947 2023-05-06 10:11:19.541457 windmill_api-1.95.1/windmill_api/models/create_draft_json_body.py
+-rw-r--r--   0        0        0      183 2023-05-06 10:11:12.089441 windmill_api-1.95.1/windmill_api/models/create_draft_json_body_typ.py
+-rw-r--r--   0        0        0     1550 2023-05-06 10:11:19.537457 windmill_api-1.95.1/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     2126 2023-05-06 10:11:19.589457 windmill_api-1.95.1/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-05-06 10:11:19.569457 windmill_api-1.95.1/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     1613 2023-05-06 10:11:19.597457 windmill_api-1.95.1/windmill_api/models/create_input.py
+-rw-r--r--   0        0        0     1171 2023-05-06 10:11:19.613457 windmill_api-1.95.1/windmill_api/models/create_input_args.py
+-rw-r--r--   0        0        0     1701 2023-05-06 10:11:19.625457 windmill_api-1.95.1/windmill_api/models/create_input_json_body.py
+-rw-r--r--   0        0        0     1217 2023-05-06 10:11:19.637457 windmill_api-1.95.1/windmill_api/models/create_input_json_body_args.py
+-rw-r--r--   0        0        0      214 2023-05-06 10:11:11.609439 windmill_api-1.95.1/windmill_api/models/create_input_runnable_type.py
+-rw-r--r--   0        0        0     2094 2023-05-06 10:11:19.661457 windmill_api-1.95.1/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-05-06 10:11:19.669457 windmill_api-1.95.1/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-05-06 10:11:19.697457 windmill_api-1.95.1/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-05-06 10:11:19.713457 windmill_api-1.95.1/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-06 10:11:19.717457 windmill_api-1.95.1/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     5120 2023-05-06 10:11:19.793458 windmill_api-1.95.1/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-05-06 10:11:12.609442 windmill_api-1.95.1/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-05-06 10:11:11.585440 windmill_api-1.95.1/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-05-06 10:11:19.741458 windmill_api-1.95.1/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-05-06 10:11:19.781458 windmill_api-1.95.1/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-05-06 10:11:19.837458 windmill_api-1.95.1/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-05-06 10:11:19.841458 windmill_api-1.95.1/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-05-06 10:11:19.861458 windmill_api-1.95.1/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-05-06 10:11:19.881458 windmill_api-1.95.1/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-05-06 10:11:19.905458 windmill_api-1.95.1/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-05-06 10:11:19.913458 windmill_api-1.95.1/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-05-06 10:11:19.929458 windmill_api-1.95.1/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-05-06 10:11:19.937458 windmill_api-1.95.1/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    11110 2023-05-06 10:11:20.069458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-05-06 10:11:19.957458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-05-06 10:11:20.025458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-05-06 10:11:20.113458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-05-06 10:11:20.097458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-05-06 10:11:20.125458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-05-06 10:11:12.161441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-05-06 10:11:20.145458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-05-06 10:11:20.193458 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-05-06 10:11:12.357441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-05-06 10:11:20.233459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-05-06 10:11:20.217459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-05-06 10:11:20.249459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-05-06 10:11:11.745440 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-05-06 10:11:20.265459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-05-06 10:11:20.285459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-05-06 10:11:11.761440 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-05-06 10:11:20.305459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-05-06 10:11:11.589439 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-05-06 10:11:12.105441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-05-06 10:11:20.333459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-05-06 10:11:20.425459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-05-06 10:11:20.373459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-05-06 10:11:20.405459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-05-06 10:11:20.441459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-05-06 10:11:20.457459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-06 10:11:11.773440 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-06 10:11:20.469459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-06 10:11:12.345441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-05-06 10:11:20.489459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-05-06 10:11:20.501459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-05-06 10:11:20.577459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-05-06 10:11:20.541459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-05-06 10:11:20.601459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-05-06 10:11:20.613459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-05-06 10:11:20.633459 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-06 10:11:12.329441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-05-06 10:11:20.645460 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-06 10:11:12.149441 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-05-06 10:11:20.661460 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-05-06 10:11:20.677460 windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-05-06 10:11:20.689459 windmill_api-1.95.1/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     7636 2023-05-06 10:11:20.805460 windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-05-06 10:11:20.709460 windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-05-06 10:11:12.161441 windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-05-06 10:11:11.665440 windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-05-06 10:11:20.733460 windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-05-06 10:11:20.777460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-06 10:11:20.841460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-06 10:11:11.757440 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-06 10:11:20.833460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-06 10:11:20.861460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-06 10:11:20.869460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-06 10:11:20.901460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-06 10:11:12.149441 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-06 10:11:20.893460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-06 10:11:20.933460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-06 10:11:12.073441 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-06 10:11:20.933460 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-06 10:11:11.933440 windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-05-06 10:11:20.957460 windmill_api-1.95.1/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-05-06 10:11:20.969460 windmill_api-1.95.1/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-05-06 10:11:21.009460 windmill_api-1.95.1/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-05-06 10:11:21.001460 windmill_api-1.95.1/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-05-06 10:11:21.025460 windmill_api-1.95.1/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-05-06 10:11:21.033460 windmill_api-1.95.1/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-05-06 10:11:21.065460 windmill_api-1.95.1/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-05-06 10:11:21.061460 windmill_api-1.95.1/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-05-06 10:11:21.093460 windmill_api-1.95.1/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-05-06 10:11:21.113460 windmill_api-1.95.1/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-05-06 10:11:21.113460 windmill_api-1.95.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-05-06 10:11:21.141461 windmill_api-1.95.1/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-05-06 10:11:21.141461 windmill_api-1.95.1/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-05-06 10:11:21.165461 windmill_api-1.95.1/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4924 2023-05-06 10:11:21.245461 windmill_api-1.95.1/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-05-06 10:11:21.185461 windmill_api-1.95.1/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3707 2023-05-06 10:11:21.237461 windmill_api-1.95.1/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-05-06 10:11:21.257461 windmill_api-1.95.1/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-05-06 10:11:21.333461 windmill_api-1.95.1/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-05-06 10:11:21.297461 windmill_api-1.95.1/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-05-06 10:11:21.329461 windmill_api-1.95.1/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-05-06 10:11:21.381461 windmill_api-1.95.1/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-05-06 10:11:21.361461 windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-05-06 10:11:12.173441 windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-05-06 10:11:21.393461 windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-05-06 10:11:11.877440 windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-05-06 10:11:21.413461 windmill_api-1.95.1/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-05-06 10:11:21.425461 windmill_api-1.95.1/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3292 2023-05-06 10:11:21.457461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-05-06 10:11:21.465461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-06 10:11:21.485461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-06 10:11:12.153441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-06 10:11:21.497461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-06 10:11:12.165441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-05-06 10:11:11.965440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-05-06 10:11:12.509441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-05-06 10:11:21.525461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-05-06 10:11:21.537461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-06 10:11:21.557461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-06 10:11:12.581442 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-06 10:11:21.569461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-06 10:11:12.409441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-05-06 10:11:11.845440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-05-06 10:11:21.589461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-05-06 10:11:21.633462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-06 10:11:21.621461 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-06 10:11:12.453441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-06 10:11:21.649462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-06 10:11:12.445441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-05-06 10:11:11.837440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-05-06 10:11:21.693462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-05-06 10:11:21.677462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-06 10:11:12.025441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-05-06 10:11:21.713462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-06 10:11:12.509441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-05-06 10:11:21.777462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-05-06 10:11:21.769462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-06 10:11:21.801462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-06 10:11:21.813462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-06 10:11:21.833462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-06 10:11:12.593442 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-06 10:11:21.845462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-06 10:11:11.581440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-06 10:11:21.861462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-06 10:11:21.877462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-05-06 10:11:11.977440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-05-06 10:11:21.901462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-05-06 10:11:21.913462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-06 10:11:21.989462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-06 10:11:21.957462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-06 10:11:21.985462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-06 10:11:22.045462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-06 10:11:22.017462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-06 10:11:11.989440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-06 10:11:22.045462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-06 10:11:11.869440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-06 10:11:22.077463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-06 10:11:22.081462 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-05-06 10:11:22.181463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-05-06 10:11:22.121463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-06 10:11:22.153463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-06 10:11:22.185463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-06 10:11:22.213463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-06 10:11:11.649440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-06 10:11:22.217463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-06 10:11:11.753440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-06 10:11:22.241463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-06 10:11:22.249463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-06 10:11:11.653440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-05-06 10:11:22.281463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-05-06 10:11:22.289463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-06 10:11:22.365463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-06 10:11:22.329463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-06 10:11:22.361463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-06 10:11:22.417463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-06 10:11:22.393463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-06 10:11:11.809440 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-06 10:11:22.425463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-06 10:11:12.101441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-06 10:11:22.449463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-06 10:11:22.457463 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-06 10:11:12.293441 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-05-06 10:11:22.477464 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-05-06 10:11:12.469442 windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-05-06 10:11:22.501464 windmill_api-1.95.1/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-05-06 10:11:22.497464 windmill_api-1.95.1/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-05-06 10:11:22.541464 windmill_api-1.95.1/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-05-06 10:11:22.617464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-05-06 10:11:22.581464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-05-06 10:11:22.609464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-05-06 10:11:22.645464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-05-06 10:11:22.649464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-06 10:11:12.169441 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-05-06 10:11:22.669464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-06 10:11:11.701440 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-05-06 10:11:22.681464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-05-06 10:11:22.697464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-05-06 10:11:22.765464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-05-06 10:11:22.741464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-05-06 10:11:22.769464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-05-06 10:11:22.797464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-05-06 10:11:22.825464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-06 10:11:11.789440 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-05-06 10:11:22.833464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-06 10:11:11.713440 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-05-06 10:11:22.857464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-05-06 10:11:22.861464 windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-05-06 10:11:22.877464 windmill_api-1.95.1/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-05-06 10:11:22.909464 windmill_api-1.95.1/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-05-06 10:11:22.961465 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-05-06 10:11:22.969465 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-05-06 10:11:22.993465 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-05-06 10:11:11.761440 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-05-06 10:11:23.001465 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-05-06 10:11:23.029465 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-05-06 10:11:12.357441 windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-05-06 10:11:23.089465 windmill_api-1.95.1/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-05-06 10:11:23.053465 windmill_api-1.95.1/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-05-06 10:11:23.081465 windmill_api-1.95.1/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-05-06 10:11:12.409441 windmill_api-1.95.1/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-05-06 10:11:23.109465 windmill_api-1.95.1/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-05-06 10:11:23.125465 windmill_api-1.95.1/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-05-06 10:11:12.437441 windmill_api-1.95.1/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-05-06 10:11:23.233465 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-05-06 10:11:23.149465 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-05-06 10:11:23.181465 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-05-06 10:11:12.085441 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-05-06 10:11:23.209465 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-05-06 10:11:23.245465 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-05-06 10:11:11.945440 windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-05-06 10:11:23.269465 windmill_api-1.95.1/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-05-06 10:11:23.285465 windmill_api-1.95.1/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-05-06 10:11:23.353465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-05-06 10:11:23.357465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-06 10:11:23.385465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-06 10:11:23.393465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-06 10:11:23.417465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-06 10:11:12.113441 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-06 10:11:23.421465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-06 10:11:12.329441 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-06 10:11:23.449465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-06 10:11:23.453465 windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-06 10:11:23.533465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-05-06 10:11:23.493465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-06 10:11:23.525465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-06 10:11:23.561465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-06 10:11:23.597465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-06 10:11:11.945440 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-06 10:11:23.593465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-06 10:11:12.129441 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-06 10:11:23.625465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-06 10:11:23.625465 windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-05-06 10:11:23.657465 windmill_api-1.95.1/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-05-06 10:11:23.645465 windmill_api-1.95.1/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-05-06 10:11:23.673465 windmill_api-1.95.1/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-05-06 10:11:23.709465 windmill_api-1.95.1/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-05-06 10:11:23.701465 windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-05-06 10:11:12.293441 windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-05-06 10:11:23.729465 windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-05-06 10:11:12.173441 windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-05-06 10:11:23.821465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-05-06 10:11:23.769465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-06 10:11:23.797465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-06 10:11:23.833465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-06 10:11:23.853465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-06 10:11:11.617440 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-06 10:11:23.861465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-06 10:11:12.533442 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-06 10:11:23.893465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-06 10:11:23.889465 windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-05-06 10:11:11.793440 windmill_api-1.95.1/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-05-06 10:11:23.941465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-05-06 10:11:12.557442 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-05-06 10:11:23.917465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-05-06 10:11:23.969465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-05-06 10:11:11.969440 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-05-06 10:11:23.993465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-05-06 10:11:23.989465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4819 2023-05-06 10:11:24.053465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0      228 2023-05-06 10:11:12.401441 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1330 2023-05-06 10:11:24.013465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3992 2023-05-06 10:11:24.061465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
+-rw-r--r--   0        0        0      234 2023-05-06 10:11:11.997440 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2160 2023-05-06 10:11:24.081465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1463 2023-05-06 10:11:24.081465 windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-05-06 10:11:24.133465 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-05-06 10:11:12.033440 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-05-06 10:11:24.109465 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-05-06 10:11:24.193465 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-05-06 10:11:12.333441 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-05-06 10:11:24.161465 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-05-06 10:11:24.181465 windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-05-06 10:11:24.229465 windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-05-06 10:11:12.181441 windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-05-06 10:11:12.457441 windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-05-06 10:11:24.221465 windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    11008 2023-05-06 10:11:24.361466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-05-06 10:11:24.249465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-05-06 10:11:24.297465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-05-06 10:11:24.409465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-05-06 10:11:24.389465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-05-06 10:11:24.421465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-05-06 10:11:11.845440 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-05-06 10:11:24.437466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-05-06 10:11:24.461465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-05-06 10:11:11.589439 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-05-06 10:11:24.521465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-05-06 10:11:24.489466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-06 10:11:24.517465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-06 10:11:12.069441 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-06 10:11:24.545466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-06 10:11:24.561466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-06 10:11:11.845440 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-05-06 10:11:24.625465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-05-06 10:11:11.861440 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-05-06 10:11:12.009441 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-05-06 10:11:24.605466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-05-06 10:11:24.689466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-05-06 10:11:24.669466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-05-06 10:11:24.697466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-05-06 10:11:24.761466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-05-06 10:11:24.729466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-05-06 10:11:11.865440 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-05-06 10:11:24.761466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-05-06 10:11:12.481442 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-05-06 10:11:24.789466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-05-06 10:11:24.793465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-05-06 10:11:24.873466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-05-06 10:11:24.837466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-06 10:11:24.865465 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-06 10:11:24.901466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-06 10:11:24.901466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-06 10:11:12.157441 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-06 10:11:24.929466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-06 10:11:12.037440 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-06 10:11:24.933466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-06 10:11:24.961466 windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5374 2023-05-06 10:11:25.045466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-05-06 10:11:24.981466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-05-06 10:11:25.001466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-05-06 10:11:25.045466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-05-06 10:11:25.129466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-05-06 10:11:25.089466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-06 10:11:25.125466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-06 10:11:25.193466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-06 10:11:25.161466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-06 10:11:11.569440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-06 10:11:25.189466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-06 10:11:11.633440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-06 10:11:25.221466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-06 10:11:25.225466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-05-06 10:11:25.305466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-05-06 10:11:25.265466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-05-06 10:11:25.297466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-05-06 10:11:25.333466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-05-06 10:11:25.333466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-06 10:11:11.577439 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-05-06 10:11:25.369466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-06 10:11:11.965440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-05-06 10:11:25.365466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-05-06 10:11:25.425466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2093 2023-05-06 10:11:25.401466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5695 2023-05-06 10:11:25.473466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0     1360 2023-05-06 10:11:25.445466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
+-rw-r--r--   0        0        0     1337 2023-05-06 10:11:25.465466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0     3559 2023-05-06 10:11:25.509466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
+-rw-r--r--   0        0        0     7829 2023-05-06 10:11:25.597466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
+-rw-r--r--   0        0        0     3606 2023-05-06 10:11:25.553466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2067 2023-05-06 10:11:25.581466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2371 2023-05-06 10:11:25.617466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2343 2023-05-06 10:11:25.629466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      205 2023-05-06 10:11:11.785440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2210 2023-05-06 10:11:25.645466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      205 2023-05-06 10:11:11.881440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2060 2023-05-06 10:11:25.661466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2111 2023-05-06 10:11:25.673466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7685 2023-05-06 10:11:25.745466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
+-rw-r--r--   0        0        0     3542 2023-05-06 10:11:25.713466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2057 2023-05-06 10:11:25.745466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2361 2023-05-06 10:11:25.777466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2323 2023-05-06 10:11:25.777466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      203 2023-05-06 10:11:11.741440 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2190 2023-05-06 10:11:25.805466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      203 2023-05-06 10:11:12.581442 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2050 2023-05-06 10:11:25.809466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2101 2023-05-06 10:11:25.837466 windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2756 2023-05-06 10:11:25.849466 windmill_api-1.95.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
+-rw-r--r--   0        0        0     1337 2023-05-06 10:11:25.857466 windmill_api-1.95.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
+-rw-r--r--   0        0        0     2010 2023-05-06 10:11:25.881466 windmill_api-1.95.1/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-05-06 10:11:25.877466 windmill_api-1.95.1/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-05-06 10:11:25.913466 windmill_api-1.95.1/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      301 2023-05-06 10:11:11.797440 windmill_api-1.95.1/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-05-06 10:11:25.905466 windmill_api-1.95.1/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-05-06 10:11:25.985466 windmill_api-1.95.1/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-05-06 10:11:25.933466 windmill_api-1.95.1/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-05-06 10:11:25.957466 windmill_api-1.95.1/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-05-06 10:11:26.017466 windmill_api-1.95.1/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-05-06 10:11:26.017466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-05-06 10:11:26.057466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-05-06 10:11:26.037466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-05-06 10:11:26.085466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-05-06 10:11:26.141466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-05-06 10:11:26.125466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-05-06 10:11:26.157466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-05-06 10:11:26.173466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-05-06 10:11:26.185466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-06 10:11:12.325441 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-05-06 10:11:26.205466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-06 10:11:11.845440 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-05-06 10:11:26.217466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-05-06 10:11:26.233466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-05-06 10:11:26.301466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-05-06 10:11:26.277466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-05-06 10:11:26.305466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-05-06 10:11:26.337466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-05-06 10:11:26.337466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-05-06 10:11:12.617442 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-05-06 10:11:26.401466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-05-06 10:11:12.401441 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-05-06 10:11:26.405466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-05-06 10:11:26.433466 windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-05-06 10:11:26.445466 windmill_api-1.95.1/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-05-06 10:11:12.561442 windmill_api-1.95.1/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     2644 2023-05-06 10:11:26.473466 windmill_api-1.95.1/windmill_api/models/get_input_history_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-05-06 10:11:26.461466 windmill_api-1.95.1/windmill_api/models/get_input_history_response_200_item_args.py
+-rw-r--r--   0        0        0      218 2023-05-06 10:11:11.941440 windmill_api-1.95.1/windmill_api/models/get_input_history_runnable_type.py
+-rw-r--r--   0        0        0     1852 2023-05-06 10:11:26.497466 windmill_api-1.95.1/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-05-06 10:11:12.113441 windmill_api-1.95.1/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-05-06 10:11:26.513466 windmill_api-1.95.1/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-05-06 10:11:26.525466 windmill_api-1.95.1/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-05-06 10:11:26.569466 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-05-06 10:11:11.585440 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-05-06 10:11:26.545466 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-05-06 10:11:26.605466 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-05-06 10:11:12.005440 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-05-06 10:11:26.597466 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-05-06 10:11:26.617466 windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-05-06 10:11:26.657466 windmill_api-1.95.1/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-06 10:11:26.641466 windmill_api-1.95.1/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-05-06 10:11:26.677466 windmill_api-1.95.1/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-05-06 10:11:26.685466 windmill_api-1.95.1/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-05-06 10:11:26.737466 windmill_api-1.95.1/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-05-06 10:11:26.705466 windmill_api-1.95.1/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-05-06 10:11:26.725466 windmill_api-1.95.1/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     7558 2023-05-06 10:11:26.865466 windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-06 10:11:26.757466 windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-06 10:11:12.613442 windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-06 10:11:12.097441 windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-06 10:11:26.825466 windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     7558 2023-05-06 10:11:26.925466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-06 10:11:26.885466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-06 10:11:12.289441 windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-06 10:11:12.113441 windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-06 10:11:26.909466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     6383 2023-05-06 10:11:26.993466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5608 2023-05-06 10:11:27.001466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0      269 2023-05-06 10:11:11.897440 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
+-rw-r--r--   0        0        0      227 2023-05-06 10:11:12.589442 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
+-rw-r--r--   0        0        0     1347 2023-05-06 10:11:27.017466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0      264 2023-05-06 10:11:11.705440 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
+-rw-r--r--   0        0        0      222 2023-05-06 10:11:12.573442 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
+-rw-r--r--   0        0        0     1319 2023-05-06 10:11:27.025466 windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-05-06 10:11:27.049466 windmill_api-1.95.1/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-05-06 10:11:27.081466 windmill_api-1.95.1/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-05-06 10:11:27.081466 windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-05-06 10:11:27.109466 windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-05-06 10:11:27.113466 windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-05-06 10:11:11.641440 windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-05-06 10:11:27.169466 windmill_api-1.95.1/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-06 10:11:27.133466 windmill_api-1.95.1/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-05-06 10:11:27.177466 windmill_api-1.95.1/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-05-06 10:11:12.013440 windmill_api-1.95.1/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-05-06 10:11:27.245466 windmill_api-1.95.1/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-05-06 10:11:27.257466 windmill_api-1.95.1/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-05-06 10:11:11.741440 windmill_api-1.95.1/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-05-06 10:11:27.289466 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-05-06 10:11:27.317466 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-05-06 10:11:12.077441 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-05-06 10:11:27.317466 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-05-06 10:11:27.341467 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-05-06 10:11:27.345466 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-05-06 10:11:27.381466 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-05-06 10:11:11.593439 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-05-06 10:11:27.373467 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-05-06 10:11:27.413467 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-05-06 10:11:11.769440 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-06 10:11:27.409467 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-06 10:11:11.989440 windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-05-06 10:11:27.453467 windmill_api-1.95.1/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-05-06 10:11:27.433467 windmill_api-1.95.1/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-05-06 10:11:27.465467 windmill_api-1.95.1/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-05-06 10:11:11.877440 windmill_api-1.95.1/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     2377 2023-05-06 10:11:27.493466 windmill_api-1.95.1/windmill_api/models/input_.py
+-rw-r--r--   0        0        0     1138 2023-05-06 10:11:27.485467 windmill_api-1.95.1/windmill_api/models/input_args.py
+-rw-r--r--   0        0        0     1820 2023-05-06 10:11:27.517467 windmill_api-1.95.1/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-05-06 10:11:12.013440 windmill_api-1.95.1/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-05-06 10:11:27.521467 windmill_api-1.95.1/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-05-06 10:11:12.461441 windmill_api-1.95.1/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-05-06 10:11:27.545467 windmill_api-1.95.1/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-05-06 10:11:27.545467 windmill_api-1.95.1/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-05-06 10:11:12.021440 windmill_api-1.95.1/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-05-06 10:11:27.581467 windmill_api-1.95.1/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-05-06 10:11:12.493441 windmill_api-1.95.1/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-05-06 10:11:27.597467 windmill_api-1.95.1/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-05-06 10:11:11.721440 windmill_api-1.95.1/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-05-06 10:11:27.641466 windmill_api-1.95.1/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-05-06 10:11:12.161441 windmill_api-1.95.1/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-05-06 10:11:27.685467 windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-05-06 10:11:12.565442 windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-05-06 10:11:12.133441 windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-05-06 10:11:27.669467 windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11220 2023-05-06 10:11:27.805467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-05-06 10:11:27.705467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-05-06 10:11:27.749467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-05-06 10:11:27.837467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-05-06 10:11:27.833467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-05-06 10:11:27.865467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-05-06 10:11:11.833440 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-05-06 10:11:27.865467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-05-06 10:11:27.901467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-05-06 10:11:12.009441 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-05-06 10:11:27.949467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-05-06 10:11:27.929467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-05-06 10:11:27.957467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-05-06 10:11:11.917440 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-05-06 10:11:27.977467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-05-06 10:11:27.997467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-05-06 10:11:12.085441 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-05-06 10:11:28.009467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-05-06 10:11:12.461441 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-05-06 10:11:12.081441 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-05-06 10:11:28.097467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-05-06 10:11:28.129467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-05-06 10:11:28.137467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-05-06 10:11:28.157467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-05-06 10:11:28.169467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-05-06 10:11:28.189467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-05-06 10:11:11.557439 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-05-06 10:11:28.201467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-05-06 10:11:12.201441 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-05-06 10:11:28.221467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-05-06 10:11:28.229467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-05-06 10:11:28.305467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-05-06 10:11:28.269467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-05-06 10:11:28.297467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-05-06 10:11:28.333467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-05-06 10:11:28.337467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-05-06 10:11:11.577439 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-05-06 10:11:28.361467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-05-06 10:11:11.885440 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-05-06 10:11:28.365467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-05-06 10:11:28.393467 windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-05-06 10:11:28.397467 windmill_api-1.95.1/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     1863 2023-05-06 10:11:28.421467 windmill_api-1.95.1/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     2074 2023-05-06 10:11:28.469467 windmill_api-1.95.1/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-06 10:11:28.441467 windmill_api-1.95.1/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-05-06 10:11:28.485467 windmill_api-1.95.1/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-05-06 10:11:28.489467 windmill_api-1.95.1/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-05-06 10:11:28.521467 windmill_api-1.95.1/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-05-06 10:11:28.529467 windmill_api-1.95.1/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-05-06 10:11:28.589467 windmill_api-1.95.1/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-05-06 10:11:28.565467 windmill_api-1.95.1/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-05-06 10:11:28.601467 windmill_api-1.95.1/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-05-06 10:11:28.629467 windmill_api-1.95.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-05-06 10:11:12.257441 windmill_api-1.95.1/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     2590 2023-05-06 10:11:28.641467 windmill_api-1.95.1/windmill_api/models/list_inputs_response_200_item.py
+-rw-r--r--   0        0        0     1250 2023-05-06 10:11:28.649467 windmill_api-1.95.1/windmill_api/models/list_inputs_response_200_item_args.py
+-rw-r--r--   0        0        0      213 2023-05-06 10:11:12.109441 windmill_api-1.95.1/windmill_api/models/list_inputs_runnable_type.py
+-rw-r--r--   0        0        0     1922 2023-05-06 10:11:28.677467 windmill_api-1.95.1/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-05-06 10:11:11.561439 windmill_api-1.95.1/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-05-06 10:11:28.681467 windmill_api-1.95.1/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    12114 2023-05-06 10:11:28.877467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-05-06 10:11:28.705467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-05-06 10:11:28.749467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-05-06 10:11:28.833467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-05-06 10:11:28.861467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-06 10:11:28.893467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-06 10:11:12.621442 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-06 10:11:28.909467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-06 10:11:28.969467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-06 10:11:12.213441 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-05-06 10:11:28.997467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-05-06 10:11:28.997467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-05-06 10:11:29.029467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-05-06 10:11:12.445441 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-05-06 10:11:29.025467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-05-06 10:11:29.061467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-05-06 10:11:11.969440 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-05-06 10:11:29.065467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-05-06 10:11:12.629442 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-05-06 10:11:12.105441 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-05-06 10:11:29.105467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-05-06 10:11:29.149467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-05-06 10:11:29.145467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-06 10:11:29.177467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-06 10:11:29.185467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-06 10:11:29.205467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-06 10:11:12.309441 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-06 10:11:29.213467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-06 10:11:11.957440 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-06 10:11:29.237467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-06 10:11:29.297467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-05-06 10:11:29.357467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-05-06 10:11:29.337467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-06 10:11:29.365467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-06 10:11:29.389467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-06 10:11:29.397467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-06 10:11:12.109441 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-06 10:11:29.421467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-06 10:11:11.849440 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-06 10:11:29.429467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-06 10:11:29.449467 windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     4884 2023-05-06 10:11:29.497467 windmill_api-1.95.1/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-06 10:11:29.469467 windmill_api-1.95.1/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-05-06 10:11:29.505467 windmill_api-1.95.1/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-05-06 10:11:29.557467 windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-05-06 10:11:29.525467 windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-05-06 10:11:29.545467 windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     7551 2023-05-06 10:11:29.641467 windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-06 10:11:29.581467 windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-06 10:11:12.389441 windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-05-06 10:11:12.385441 windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-05-06 10:11:29.605467 windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-05-06 10:11:29.649467 windmill_api-1.95.1/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-05-06 10:11:29.673467 windmill_api-1.95.1/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-05-06 10:11:29.677467 windmill_api-1.95.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-05-06 10:11:29.713467 windmill_api-1.95.1/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-05-06 10:11:12.405441 windmill_api-1.95.1/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4307 2023-05-06 10:11:29.789467 windmill_api-1.95.1/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-05-06 10:11:29.785467 windmill_api-1.95.1/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-05-06 10:11:29.849467 windmill_api-1.95.1/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-06 10:11:29.809467 windmill_api-1.95.1/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-05-06 10:11:29.849467 windmill_api-1.95.1/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-05-06 10:11:29.885467 windmill_api-1.95.1/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-05-06 10:11:29.885467 windmill_api-1.95.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-05-06 10:11:29.917467 windmill_api-1.95.1/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-05-06 10:11:29.929467 windmill_api-1.95.1/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-05-06 10:11:12.197441 windmill_api-1.95.1/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-05-06 10:11:29.941467 windmill_api-1.95.1/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-05-06 10:11:29.997467 windmill_api-1.95.1/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-05-06 10:11:29.961467 windmill_api-1.95.1/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-05-06 10:11:30.029467 windmill_api-1.95.1/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-05-06 10:11:30.013467 windmill_api-1.95.1/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-05-06 10:11:30.041467 windmill_api-1.95.1/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-05-06 10:11:30.057467 windmill_api-1.95.1/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-05-06 10:11:30.069467 windmill_api-1.95.1/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-05-06 10:11:30.097468 windmill_api-1.95.1/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-05-06 10:11:30.173467 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-05-06 10:11:12.217441 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-05-06 10:11:30.125467 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-05-06 10:11:30.149467 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-05-06 10:11:30.229467 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-05-06 10:11:30.209468 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-05-06 10:11:11.685440 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-06 10:11:30.237467 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-05-06 10:11:30.265468 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-05-06 10:11:11.721440 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-05-06 10:11:30.261468 windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-06 10:11:11.685440 windmill_api-1.95.1/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-05-06 10:11:30.305467 windmill_api-1.95.1/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-05-06 10:11:30.289467 windmill_api-1.95.1/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     4866 2023-05-06 10:11:30.361467 windmill_api-1.95.1/windmill_api/models/new_script.py
+-rw-r--r--   0        0        0      238 2023-05-06 10:11:12.261441 windmill_api-1.95.1/windmill_api/models/new_script_kind.py
+-rw-r--r--   0        0        0      196 2023-05-06 10:11:12.413441 windmill_api-1.95.1/windmill_api/models/new_script_language.py
+-rw-r--r--   0        0        0     1171 2023-05-06 10:11:30.329467 windmill_api-1.95.1/windmill_api/models/new_script_schema.py
+-rw-r--r--   0        0        0     5879 2023-05-06 10:11:30.413468 windmill_api-1.95.1/windmill_api/models/new_script_with_draft.py
+-rw-r--r--   0        0        0     5192 2023-05-06 10:11:30.433467 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft.py
+-rw-r--r--   0        0        0      252 2023-05-06 10:11:11.889440 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft_kind.py
+-rw-r--r--   0        0        0      210 2023-05-06 10:11:11.961440 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft_language.py
+-rw-r--r--   0        0        0     1250 2023-05-06 10:11:30.441468 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft_schema.py
+-rw-r--r--   0        0        0      247 2023-05-06 10:11:11.613440 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_kind.py
+-rw-r--r--   0        0        0      205 2023-05-06 10:11:11.957440 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_language.py
+-rw-r--r--   0        0        0     1222 2023-05-06 10:11:30.457468 windmill_api-1.95.1/windmill_api/models/new_script_with_draft_schema.py
+-rw-r--r--   0        0        0     2108 2023-05-06 10:11:30.473467 windmill_api-1.95.1/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-05-06 10:11:30.497468 windmill_api-1.95.1/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-05-06 10:11:30.505468 windmill_api-1.95.1/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-05-06 10:11:30.537468 windmill_api-1.95.1/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-05-06 10:11:30.525468 windmill_api-1.95.1/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-05-06 10:11:30.613468 windmill_api-1.95.1/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-05-06 10:11:30.665468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-05-06 10:11:30.653468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-05-06 10:11:30.685468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-05-06 10:11:30.701468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-05-06 10:11:30.713468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-05-06 10:11:11.865440 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-05-06 10:11:30.729468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-05-06 10:11:12.477441 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-05-06 10:11:30.745468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-05-06 10:11:30.757468 windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-05-06 10:11:30.825469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-05-06 10:11:30.797469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-05-06 10:11:30.829469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-05-06 10:11:30.861469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-05-06 10:11:30.861469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-06 10:11:12.281441 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-05-06 10:11:30.889469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-06 10:11:11.701440 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-05-06 10:11:30.889469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-05-06 10:11:30.917469 windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-05-06 10:11:30.933469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-05-06 10:11:30.937469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-05-06 10:11:31.021469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-05-06 10:11:31.065469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-05-06 10:11:31.061469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-05-06 10:11:31.093469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-05-06 10:11:31.101469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-05-06 10:11:31.121469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-05-06 10:11:11.789440 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-05-06 10:11:31.129469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-06 10:11:11.757440 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-05-06 10:11:31.153469 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-05-06 10:11:31.161470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-05-06 10:11:31.233470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-05-06 10:11:31.201470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-05-06 10:11:31.233470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-05-06 10:11:31.265470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-05-06 10:11:31.261470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-06 10:11:12.165441 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-05-06 10:11:31.293470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-06 10:11:12.581442 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-05-06 10:11:31.297470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-05-06 10:11:31.321470 windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-05-06 10:11:31.329470 windmill_api-1.95.1/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-05-06 10:11:31.357470 windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-05-06 10:11:31.357470 windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-06 10:11:11.825440 windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-05-06 10:11:31.429470 windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-06 10:11:11.681440 windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-05-06 10:11:11.877440 windmill_api-1.95.1/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-05-06 10:11:31.397470 windmill_api-1.95.1/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-05-06 10:11:31.433470 windmill_api-1.95.1/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-05-06 10:11:31.457470 windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-06 10:11:12.505442 windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-05-06 10:11:31.465470 windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-06 10:11:12.121441 windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-05-06 10:11:12.145441 windmill_api-1.95.1/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-05-06 10:11:31.509470 windmill_api-1.95.1/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-05-06 10:11:12.593442 windmill_api-1.95.1/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-05-06 10:11:31.489470 windmill_api-1.95.1/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-05-06 10:11:31.513470 windmill_api-1.95.1/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2359 2023-05-06 10:11:31.545470 windmill_api-1.95.1/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-05-06 10:11:31.533470 windmill_api-1.95.1/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-05-06 10:11:12.433441 windmill_api-1.95.1/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-05-06 10:11:31.561470 windmill_api-1.95.1/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-05-06 10:11:31.589470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-05-06 10:11:31.625470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-05-06 10:11:11.689440 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-05-06 10:11:31.613470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-05-06 10:11:31.641470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-05-06 10:11:31.701470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-05-06 10:11:31.677470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-05-06 10:11:12.357441 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-05-06 10:11:31.705470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-05-06 10:11:31.741470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-05-06 10:11:11.573439 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-05-06 10:11:31.733470 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-05-06 10:11:12.525442 windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11580 2023-05-06 10:11:31.937471 windmill_api-1.95.1/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-05-06 10:11:31.761470 windmill_api-1.95.1/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-05-06 10:11:31.805470 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-05-06 10:11:31.889470 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-05-06 10:11:31.917471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-05-06 10:11:31.949471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-05-06 10:11:12.145441 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-05-06 10:11:31.965470 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-05-06 10:11:31.985471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-05-06 10:11:12.165441 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-05-06 10:11:32.049471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-05-06 10:11:32.013471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-05-06 10:11:32.041471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-05-06 10:11:11.769440 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-05-06 10:11:32.069471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-05-06 10:11:32.085471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-05-06 10:11:11.565440 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-05-06 10:11:32.157471 windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-05-06 10:11:12.417441 windmill_api-1.95.1/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-05-06 10:11:11.901440 windmill_api-1.95.1/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-05-06 10:11:32.129471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-05-06 10:11:32.277471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-05-06 10:11:32.201471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-05-06 10:11:32.229471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-05-06 10:11:32.265471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-05-06 10:11:32.297471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-06 10:11:12.269441 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-05-06 10:11:32.305471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-06 10:11:12.201441 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-05-06 10:11:32.325471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-05-06 10:11:32.333471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-05-06 10:11:32.409471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-05-06 10:11:32.373471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-05-06 10:11:32.405471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-05-06 10:11:32.437471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-05-06 10:11:32.437471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-06 10:11:12.409441 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-05-06 10:11:32.465471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-06 10:11:12.097441 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-05-06 10:11:32.469471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-05-06 10:11:32.497471 windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3028 2023-05-06 10:11:32.513471 windmill_api-1.95.1/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-05-06 10:11:32.589471 windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-05-06 10:11:32.541471 windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-05-06 10:11:12.113441 windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-05-06 10:11:32.573471 windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-05-06 10:11:12.057441 windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-05-06 10:11:12.521442 windmill_api-1.95.1/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-05-06 10:11:11.585440 windmill_api-1.95.1/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-05-06 10:11:32.597471 windmill_api-1.95.1/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-05-06 10:11:32.613471 windmill_api-1.95.1/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      304 2023-05-06 10:11:11.937440 windmill_api-1.95.1/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-05-06 10:11:32.625471 windmill_api-1.95.1/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-05-06 10:11:32.637471 windmill_api-1.95.1/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-05-06 10:11:32.677471 windmill_api-1.95.1/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-05-06 10:11:32.657471 windmill_api-1.95.1/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-05-06 10:11:32.693471 windmill_api-1.95.1/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-05-06 10:11:32.697471 windmill_api-1.95.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-06 10:11:32.717471 windmill_api-1.95.1/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-05-06 10:11:32.737471 windmill_api-1.95.1/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-05-06 10:11:32.745471 windmill_api-1.95.1/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-05-06 10:11:32.769472 windmill_api-1.95.1/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-05-06 10:11:32.765472 windmill_api-1.95.1/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-05-06 10:11:32.801472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-05-06 10:11:32.789471 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-05-06 10:11:32.897472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-05-06 10:11:32.885472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-05-06 10:11:32.925472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-05-06 10:11:32.925472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-05-06 10:11:32.961472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-05-06 10:11:32.957472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-06 10:11:11.729440 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-05-06 10:11:32.985472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-06 10:11:11.673440 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-05-06 10:11:32.989472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-05-06 10:11:33.017472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-05-06 10:11:33.145472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-05-06 10:11:33.057472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-05-06 10:11:33.089472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-05-06 10:11:33.121472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-05-06 10:11:33.153472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-06 10:11:12.465442 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-05-06 10:11:33.173472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-06 10:11:12.301441 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-05-06 10:11:33.181472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-05-06 10:11:33.205472 windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-05-06 10:11:33.205472 windmill_api-1.95.1/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-05-06 10:11:33.225472 windmill_api-1.95.1/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2634 2023-05-06 10:11:33.241472 windmill_api-1.95.1/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-05-06 10:11:33.245472 windmill_api-1.95.1/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-05-06 10:11:12.385441 windmill_api-1.95.1/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-05-06 10:11:33.265472 windmill_api-1.95.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-05-06 10:11:33.265472 windmill_api-1.95.1/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0      203 2023-05-06 10:11:12.341441 windmill_api-1.95.1/windmill_api/models/runnable_type.py
+-rw-r--r--   0        0        0     4086 2023-05-06 10:11:33.325472 windmill_api-1.95.1/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-05-06 10:11:33.289472 windmill_api-1.95.1/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-05-06 10:11:33.309472 windmill_api-1.95.1/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     7003 2023-05-06 10:11:33.465472 windmill_api-1.95.1/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-05-06 10:11:33.345472 windmill_api-1.95.1/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-05-06 10:11:33.365472 windmill_api-1.95.1/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-05-06 10:11:12.269441 windmill_api-1.95.1/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-05-06 10:11:12.473441 windmill_api-1.95.1/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-05-06 10:11:33.389472 windmill_api-1.95.1/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-05-06 10:11:33.413472 windmill_api-1.95.1/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-05-06 10:11:33.437472 windmill_api-1.95.1/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-05-06 10:11:33.469472 windmill_api-1.95.1/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-05-06 10:11:33.489472 windmill_api-1.95.1/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-05-06 10:11:33.505472 windmill_api-1.95.1/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      185 2023-05-06 10:11:12.397441 windmill_api-1.95.1/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-05-06 10:11:33.521472 windmill_api-1.95.1/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-05-06 10:11:12.181441 windmill_api-1.95.1/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-05-06 10:11:33.545472 windmill_api-1.95.1/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-05-06 10:11:33.565472 windmill_api-1.95.1/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-05-06 10:11:33.581472 windmill_api-1.95.1/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      187 2023-05-06 10:11:12.357441 windmill_api-1.95.1/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-05-06 10:11:33.613473 windmill_api-1.95.1/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-06 10:11:33.629473 windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-06 10:11:12.013440 windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-06 10:11:33.637472 windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-06 10:11:33.717473 windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-05-06 10:11:33.681473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-05-06 10:11:33.701473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-05-06 10:11:33.745473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-05-06 10:11:33.801473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-05-06 10:11:33.793473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-05-06 10:11:33.825473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-05-06 10:11:33.833473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-05-06 10:11:33.909473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-06 10:11:12.369441 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-05-06 10:11:33.861473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-06 10:11:12.509441 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-05-06 10:11:33.893473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-05-06 10:11:33.925473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-05-06 10:11:33.993473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-05-06 10:11:33.969473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-05-06 10:11:33.997473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-05-06 10:11:34.029473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-05-06 10:11:34.029473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-05-06 10:11:12.093441 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-05-06 10:11:34.057473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-05-06 10:11:12.273441 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-05-06 10:11:34.057473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-05-06 10:11:34.085473 windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-05-06 10:11:34.093473 windmill_api-1.95.1/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-05-06 10:11:34.109473 windmill_api-1.95.1/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     1670 2023-05-06 10:11:34.121473 windmill_api-1.95.1/windmill_api/models/update_input.py
+-rw-r--r--   0        0        0     1716 2023-05-06 10:11:34.141473 windmill_api-1.95.1/windmill_api/models/update_input_json_body.py
+-rw-r--r--   0        0        0     2036 2023-05-06 10:11:34.153473 windmill_api-1.95.1/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-05-06 10:11:34.169473 windmill_api-1.95.1/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-05-06 10:11:34.181473 windmill_api-1.95.1/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-05-06 10:11:34.197473 windmill_api-1.95.1/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-06 10:11:34.201473 windmill_api-1.95.1/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-05-06 10:11:34.233473 windmill_api-1.95.1/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-05-06 10:11:34.237473 windmill_api-1.95.1/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-05-06 10:11:34.257473 windmill_api-1.95.1/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     4071 2023-05-06 10:11:34.301473 windmill_api-1.95.1/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-05-06 10:11:34.281473 windmill_api-1.95.1/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-05-06 10:11:34.313473 windmill_api-1.95.1/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-05-06 10:11:34.329473 windmill_api-1.95.1/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     4222 2023-05-06 10:11:34.449473 windmill_api-1.95.1/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-05-06 10:11:34.353473 windmill_api-1.95.1/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     4211 2023-05-06 10:11:34.473473 windmill_api-1.95.1/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-05-06 10:11:34.473473 windmill_api-1.95.1/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-05-06 10:11:34.513474 windmill_api-1.95.1/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-05-06 10:11:34.509473 windmill_api-1.95.1/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-05-06 10:11:34.537474 windmill_api-1.95.1/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-05-06 10:11:01.929416 windmill_api-1.95.1/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-05-06 10:11:34.529474 windmill_api-1.95.1/windmill_api/types.py
+-rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 windmill_api-1.95.1/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.95.1/PKG-INFO
```

### Comparing `windmill_api-1.95.0/LICENSE` & `windmill_api-1.95.1/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/README.md` & `windmill_api-1.95.1/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/pyproject.toml` & `windmill_api-1.95.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windmill-api"
-version = "1.95.0"
+version = "1.95.1"
 description = "A client library for accessing Windmill API"
 license = "Apache-2.0"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
 readme = "README.md"
 packages = [
```

### Comparing `windmill_api-1.95.0/windmill_api/api/app/create_app.py` & `windmill_api-1.95.1/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/delete_app.py` & `windmill_api-1.95.1/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/execute_component.py` & `windmill_api-1.95.1/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/exists_app.py` & `windmill_api-1.95.1/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.95.1/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/get_app_by_path_with_draft.py` & `windmill_api-1.95.1/windmill_api/api/app/get_app_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.95.1/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.95.1/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.95.1/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.95.1/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/list_apps.py` & `windmill_api-1.95.1/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.95.1/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/app/update_app.py` & `windmill_api-1.95.1/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.95.1/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.95.1/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/capture/create_capture.py` & `windmill_api-1.95.1/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/capture/get_capture.py` & `windmill_api-1.95.1/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/capture/update_capture.py` & `windmill_api-1.95.1/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/draft/create_draft.py` & `windmill_api-1.95.1/windmill_api/api/draft/create_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/favorite/star.py` & `windmill_api-1.95.1/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/favorite/unstar.py` & `windmill_api-1.95.1/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.95.1/windmill_api/api/flow/archive_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/create_flow.py` & `windmill_api-1.95.1/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.95.1/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.95.1/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.95.1/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/get_flow_by_path_with_draft.py` & `windmill_api-1.95.1/windmill_api/api/flow/get_flow_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/get_flow_input_history_by_path.py` & `windmill_api-1.95.1/windmill_api/api/flow/get_flow_input_history_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.95.1/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.95.1/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/list_flows.py` & `windmill_api-1.95.1/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.95.1/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/flow/update_flow.py` & `windmill_api-1.95.1/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.95.1/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/folder/create_folder.py` & `windmill_api-1.95.1/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.95.1/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/folder/get_folder.py` & `windmill_api-1.95.1/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.95.1/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.95.1/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/folder/list_folders.py` & `windmill_api-1.95.1/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.95.1/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/folder/update_folder.py` & `windmill_api-1.95.1/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.95.1/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.95.1/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.95.1/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.95.1/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/group/create_group.py` & `windmill_api-1.95.1/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/group/delete_group.py` & `windmill_api-1.95.1/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/group/get_group.py` & `windmill_api-1.95.1/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/group/list_group_names.py` & `windmill_api-1.95.1/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/group/list_groups.py` & `windmill_api-1.95.1/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.95.1/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/group/update_group.py` & `windmill_api-1.95.1/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/input_/create_input.py` & `windmill_api-1.95.1/windmill_api/api/input_/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/input_/delete_input.py` & `windmill_api-1.95.1/windmill_api/api/input_/delete_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/input_/get_input_history.py` & `windmill_api-1.95.1/windmill_api/api/input_/get_input_history.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/input_/list_inputs.py` & `windmill_api-1.95.1/windmill_api/api/input_/list_inputs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/input_/update_input.py` & `windmill_api-1.95.1/windmill_api/api/input_/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.95.1/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.95.1/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.95.1/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.95.1/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.95.1/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.95.1/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.95.1/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.95.1/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/get_job.py` & `windmill_api-1.95.1/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.95.1/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.95.1/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.95.1/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.95.1/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/list_jobs.py` & `windmill_api-1.95.1/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/list_queue.py` & `windmill_api-1.95.1/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/result_by_id.py` & `windmill_api-1.95.1/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.95.1/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.95.1/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.95.1/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.95.1/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.95.1/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.95.1/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.95.1/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.95.1/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/run_wait_result_flow_by_path.py` & `windmill_api-1.95.1/windmill_api/api/job/run_wait_result_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.95.1/windmill_api/api/job/run_wait_result_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/job/run_wait_result_script_by_path_get.py` & `windmill_api-1.95.1/windmill_api/api/job/run_wait_result_script_by_path_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.95.1/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.95.1/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/oauth/create_account.py` & `windmill_api-1.95.1/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.95.1/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.95.1/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.95.1/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.95.1/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.95.1/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/create_resource.py` & `windmill_api-1.95.1/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.95.1/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.95.1/windmill_api/api/resource/delete_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.95.1/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.95.1/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.95.1/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/get_resource.py` & `windmill_api-1.95.1/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.95.1/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.95.1/windmill_api/api/resource/get_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/list_resource.py` & `windmill_api-1.95.1/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.95.1/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.95.1/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/update_resource.py` & `windmill_api-1.95.1/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.95.1/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.95.1/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.95.1/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.95.1/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.95.1/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.95.1/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.95.1/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.95.1/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.95.1/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.95.1/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.95.1/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.95.1/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.95.1/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/create_script.py` & `windmill_api-1.95.1/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.95.1/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.95.1/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.95.1/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.95.1/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.95.1/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.95.1/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.95.1/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.95.1/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/get_script_by_path_with_draft.py` & `windmill_api-1.95.1/windmill_api/api/script/get_script_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.95.1/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.95.1/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.95.1/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.95.1/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/list_scripts.py` & `windmill_api-1.95.1/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.95.1/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.95.1/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.95.1/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/script/raw_script_by_path_tokened.py` & `windmill_api-1.95.1/windmill_api/api/script/raw_script_by_path_tokened.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/settings/backend_version.py` & `windmill_api-1.95.1/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.95.1/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/accept_invite.py` & `windmill_api-1.95.1/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/create_token.py` & `windmill_api-1.95.1/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/create_token_impersonate.py` & `windmill_api-1.95.1/windmill_api/api/user/create_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/create_user.py` & `windmill_api-1.95.1/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.95.1/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/decline_invite.py` & `windmill_api-1.95.1/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/delete_token.py` & `windmill_api-1.95.1/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/delete_user.py` & `windmill_api-1.95.1/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/get_current_email.py` & `windmill_api-1.95.1/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/get_usage.py` & `windmill_api-1.95.1/windmill_api/api/user/get_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.95.1/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/global_user_update.py` & `windmill_api-1.95.1/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/global_whoami.py` & `windmill_api-1.95.1/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.95.1/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.95.1/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/list_tokens.py` & `windmill_api-1.95.1/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/list_usernames.py` & `windmill_api-1.95.1/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/list_users.py` & `windmill_api-1.95.1/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.95.1/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.95.1/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/login.py` & `windmill_api-1.95.1/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.95.1/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/logout.py` & `windmill_api-1.95.1/windmill_api/api/user/logout.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/set_password.py` & `windmill_api-1.95.1/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/update_user.py` & `windmill_api-1.95.1/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/whoami.py` & `windmill_api-1.95.1/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/user/whois.py` & `windmill_api-1.95.1/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/variable/create_variable.py` & `windmill_api-1.95.1/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.95.1/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.95.1/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/variable/get_variable.py` & `windmill_api-1.95.1/windmill_api/api/variable/get_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.95.1/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/variable/list_variable.py` & `windmill_api-1.95.1/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/variable/update_variable.py` & `windmill_api-1.95.1/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/worker/get_custom_tags.py` & `windmill_api-1.95.1/windmill_api/api/worker/get_custom_tags.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/worker/list_workers.py` & `windmill_api-1.95.1/windmill_api/api/worker/list_workers.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/add_user.py` & `windmill_api-1.95.1/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.95.1/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.95.1/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.95.1/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.95.1/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.95.1/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.95.1/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.95.1/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.95.1/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.95.1/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.95.1/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.95.1/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.95.1/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.95.1/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.95.1/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.95.1/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/list_workspaces.py` & `windmill_api-1.95.1/windmill_api/api/workspace/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py` & `windmill_api-1.95.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.95.1/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/client.py` & `windmill_api-1.95.1/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.95.1/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.95.1/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.95.1/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/add_user_json_body.py` & `windmill_api-1.95.1/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.95.1/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/app_with_last_version.py` & `windmill_api-1.95.1/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.95.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft.py` & `windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft_policy.py` & `windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py` & `windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py` & `windmill_api-1.95.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/archive_flow_by_path_json_body.py` & `windmill_api-1.95.1/windmill_api/models/archive_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.95.1/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/audit_log.py` & `windmill_api-1.95.1/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/audit_log_operation.py` & `windmill_api-1.95.1/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.95.1/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.95.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_all.py` & `windmill_api-1.95.1/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one.py` & `windmill_api-1.95.1/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.95.1/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.95.1/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job.py` & `windmill_api-1.95.1/windmill_api/models/completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_args.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.95.1/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.95.1/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.95.1/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/contextual_variable.py` & `windmill_api-1.95.1/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_account_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_app_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.95.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_draft_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_draft_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_group_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_input.py` & `windmill_api-1.95.1/windmill_api/models/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_input_args.py` & `windmill_api-1.95.1/windmill_api/models/create_input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_input_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_input_json_body_args.py` & `windmill_api-1.95.1/windmill_api/models/create_input_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_resource.py` & `windmill_api-1.95.1/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.95.1/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_script_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_script_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.95.1/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_token_impersonate_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_token_impersonate_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_token_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_user_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_variable.py` & `windmill_api-1.95.1/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_workspace.py` & `windmill_api-1.95.1/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.95.1/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.95.1/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.95.1/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.95.1/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.95.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.95.1/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/edit_resource.py` & `windmill_api-1.95.1/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/edit_resource_type.py` & `windmill_api-1.95.1/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/edit_schedule.py` & `windmill_api-1.95.1/windmill_api/models/edit_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.95.1/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.95.1/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/edit_variable.py` & `windmill_api-1.95.1/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.95.1/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.95.1/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.95.1/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.95.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.95.1/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.95.1/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.95.1/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow.py` & `windmill_api-1.95.1/windmill_api/models/flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_metadata.py` & `windmill_api-1.95.1/windmill_api/models/flow_metadata.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module.py` & `windmill_api-1.95.1/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.95.1/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_args.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_schema.py` & `windmill_api-1.95.1/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status.py` & `windmill_api-1.95.1/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_module.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_status_retry.py` & `windmill_api-1.95.1/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value.py` & `windmill_api-1.95.1/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/folder.py` & `windmill_api-1.95.1/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.95.1/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.95.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.95.1/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py` & `windmill_api-1.95.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_group_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_input_history_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/get_input_history_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_input_history_response_200_item_args.py` & `windmill_api-1.95.1/windmill_api/models/get_input_history_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_job_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.95.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_schedule_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.95.1/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.95.1/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.95.1/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py` & `windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py` & `windmill_api-1.95.1/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.95.1/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.95.1/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/global_user_info.py` & `windmill_api-1.95.1/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.95.1/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.95.1/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.95.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/group.py` & `windmill_api-1.95.1/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/group_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/identity.py` & `windmill_api-1.95.1/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/input_.py` & `windmill_api-1.95.1/windmill_api/models/input_.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/input_args.py` & `windmill_api-1.95.1/windmill_api/models/input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.95.1/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.95.1/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.95.1/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/javascript_transform.py` & `windmill_api-1.95.1/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/job.py` & `windmill_api-1.95.1/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.95.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_flows_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.95.1/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.95.1/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.95.1/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.95.1/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.95.1/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.95.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_inputs_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_inputs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_inputs_response_200_item_args.py` & `windmill_api-1.95.1/windmill_api/models/list_inputs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.95.1/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.95.1/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.95.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_users_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.95.1/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.95.1/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/listable_app.py` & `windmill_api-1.95.1/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/listable_resource.py` & `windmill_api-1.95.1/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/listable_variable.py` & `windmill_api-1.95.1/windmill_api/models/listable_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/login.py` & `windmill_api-1.95.1/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/login_json_body.py` & `windmill_api-1.95.1/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.95.1/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/main_arg_signature.py` & `windmill_api-1.95.1/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.95.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_schedule.py` & `windmill_api-1.95.1/windmill_api/models/new_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_schedule_args.py` & `windmill_api-1.95.1/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_script.py` & `windmill_api-1.95.1/windmill_api/models/new_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_script_schema.py` & `windmill_api-1.95.1/windmill_api/models/new_script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_script_with_draft.py` & `windmill_api-1.95.1/windmill_api/models/new_script_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_script_with_draft_draft.py` & `windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_script_with_draft_draft_schema.py` & `windmill_api-1.95.1/windmill_api/models/new_script_with_draft_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_script_with_draft_schema.py` & `windmill_api-1.95.1/windmill_api/models/new_script_with_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_token.py` & `windmill_api-1.95.1/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_token_impersonate.py` & `windmill_api-1.95.1/windmill_api/models/new_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/new_user.py` & `windmill_api-1.95.1/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow.py` & `windmill_api-1.95.1/windmill_api/models/open_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_schema.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/path_flow.py` & `windmill_api-1.95.1/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.95.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/path_script.py` & `windmill_api-1.95.1/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.95.1/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.95.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/policy.py` & `windmill_api-1.95.1/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/policy_triggerables.py` & `windmill_api-1.95.1/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.95.1/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/preview.py` & `windmill_api-1.95.1/windmill_api/models/preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/preview_args.py` & `windmill_api-1.95.1/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.95.1/windmill_api/models/preview_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.95.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job.py` & `windmill_api-1.95.1/windmill_api/models/queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_args.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/raw_script.py` & `windmill_api-1.95.1/windmill_api/models/raw_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.95.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.95.1/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.95.1/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.95.1/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.95.1/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/resource.py` & `windmill_api-1.95.1/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/resource_type.py` & `windmill_api-1.95.1/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.95.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.95.1/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/retry.py` & `windmill_api-1.95.1/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.95.1/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.95.1/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.95.1/windmill_api/models/run_script_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.95.1/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.95.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.95.1/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/schedule.py` & `windmill_api-1.95.1/windmill_api/models/schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/schedule_args.py` & `windmill_api-1.95.1/windmill_api/models/schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/schedule_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/script.py` & `windmill_api-1.95.1/windmill_api/models/script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/script_args.py` & `windmill_api-1.95.1/windmill_api/models/script_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/script_extra_perms.py` & `windmill_api-1.95.1/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/script_schema.py` & `windmill_api-1.95.1/windmill_api/models/script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/set_password_json_body.py` & `windmill_api-1.95.1/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.95.1/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/slack_token.py` & `windmill_api-1.95.1/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/slack_token_bot.py` & `windmill_api-1.95.1/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/star_json_body.py` & `windmill_api-1.95.1/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/static_transform.py` & `windmill_api-1.95.1/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/token_response.py` & `windmill_api-1.95.1/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/truncated_token.py` & `windmill_api-1.95.1/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/unstar_json_body.py` & `windmill_api-1.95.1/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_app_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.95.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.95.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_group_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_input.py` & `windmill_api-1.95.1/windmill_api/models/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_input_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_resource_type_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_resource_value_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_schedule_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.95.1/windmill_api/models/update_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_user_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/update_variable_json_body.py` & `windmill_api-1.95.1/windmill_api/models/update_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/usage.py` & `windmill_api-1.95.1/windmill_api/models/usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/user.py` & `windmill_api-1.95.1/windmill_api/models/user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/user_usage.py` & `windmill_api-1.95.1/windmill_api/models/user_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/user_workspace_list.py` & `windmill_api-1.95.1/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.95.1/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/whoami_response_200.py` & `windmill_api-1.95.1/windmill_api/models/whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/whoami_response_200_usage.py` & `windmill_api-1.95.1/windmill_api/models/whoami_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/whois_response_200.py` & `windmill_api-1.95.1/windmill_api/models/whois_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/whois_response_200_usage.py` & `windmill_api-1.95.1/windmill_api/models/whois_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/worker_ping.py` & `windmill_api-1.95.1/windmill_api/models/worker_ping.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/workspace.py` & `windmill_api-1.95.1/windmill_api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/models/workspace_invite.py` & `windmill_api-1.95.1/windmill_api/models/workspace_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/windmill_api/types.py` & `windmill_api-1.95.1/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.95.0/setup.py` & `windmill_api-1.95.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.95.0',
+    'version': '1.95.1',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.95.0/PKG-INFO` & `windmill_api-1.95.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.95.0
+Version: 1.95.1
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

