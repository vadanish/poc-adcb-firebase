# poc-adcb-firebase-version_1.0.5

deploy_to_huawei_app_gallery
[02:07:39]: --- Step: huawei_appgallery_connect_get_app_id ---
[02:07:39]: --------------------------------------------------
[02:07:39]: Fetching app access token
[02:07:40]: Fetching App ID
[02:07:40]: Successfully getting app id
[02:07:40]: Huawei app_id: 117330571
[02:07:40]: ---------------------------------------
[02:07:40]: --- Step: huawei_appgallery_connect ---
[02:07:40]: ---------------------------------------
[02:07:40]: Fetching app access token
[02:07:41]: Fetching upload URL
[02:07:43]: Uploading app
[02:08:02]: Upload app to AppGallery Connect successful
[02:08:02]: Saving app information
+------------------------------------------------------------------+
|                           Lane Context                           |
+---------------------------+--------------------------------------+
| PLATFORM_NAME             | android                              |
| LANE_NAME                 | android deploy_to_huawei_app_gallery |
| ANDROID_APPGALLERY_APP_ID | 117330571                            |
+---------------------------+--------------------------------------+
[02:08:04]: Called from Fastfile at line 161
[02:08:04]: ```
[02:08:04]:     159:	        UI.message("Huawei app_id: #{app_id}")
[02:08:04]:     160:	
[02:08:04]:  => 161:	        huawei_appgallery_connect(
[02:08:04]:     162:	            client_id: @ANDROID_HUAWEI_CLIENT_ID,
[02:08:04]:     163:	            client_secret: @ANDROID_HUAWEI_CLIENT_SECRET,
[02:08:04]: ```
[02:08:04]: {"ret"=>{"code"=>204144647, "msg"=>"[cds]update service failed, additional msg is [The new service has can't be edited service,which can't be updated!]"}}

+-----------------------------------------------------------+
|                     fastlane summary                      |
+------+--------------------------------------+-------------+
| Step | Action                               | Time (in s) |
+------+--------------------------------------+-------------+
| 1    | opt_out_usage                        | 0           |
| 2    | huawei_appgallery_connect_get_app_id | 1           |
| 💥   | huawei_appgallery_connect            | 23          |
+------+--------------------------------------+-------------+

+-----------------------------------------------------------+
|                 Plugin updates available                  |

+---------------------------+--------------+----------------+
| Plugin                    | Your Version | Latest Version |
+---------------------------+--------------+----------------+
[!] {"ret"=>{"code"=>204144647, "msg"=>"[cds]update service failed, additional msg is [The new service has can't be edited service,which can't be updated!]"}}
| firebase_app_distribution | 0.10.1       | 1.0.0          |
+---------------------------+--------------+----------------+
[02:08:04]: To update all plugins, just run
[02:08:04]: $ bundle exec fastlane update_plugins

[02:08:04]: fastlane finished with errors
