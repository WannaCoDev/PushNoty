# PushNoty
OneSignal integration with [ImpressPages CMS](https://www.impresspages.org/) Grid system. 

Create a OneSignal account if you haven't already https://onesignal.com/ 
Reaching visitors is simple with push notifications. Visitors who subscribe to get notifications from your website will get push notifications that you send. either new products you put out for sale or new content.

OneSignal is a great service but complicated to manage. If you need a Content Manager to take care of that task simply add this plugin and let them handle it for you.

once installed it'll  appear in your ImpressPages CMS admin munu
 
![image](https://cloud.githubusercontent.com/assets/7078331/24985522/ffa4d526-1fb1-11e7-9a19-10325656c2fa.png)

It is managed via the ImpressPages Grid system
 
![image](https://cloud.githubusercontent.com/assets/7078331/24985521/f98fb20a-1fb1-11e7-998b-8ea942ff1c34.png)

 And it'll be logged and pushed accordingly by OneSignal 

![image](https://cloud.githubusercontent.com/assets/7078331/24985514/e613a9c0-1fb1-11e7-842c-f789e527a89d.png)

 ##Installation


 Save
 1. Configure OneSignal settings


CHROME, FIREFOX


Go to App Settings and click Configure for the Google Chrome platform
 
![image](https://cloud.githubusercontent.com/assets/7078331/24985568/523bf6ca-1fb2-11e7-82e3-e9b6712bed7e.png)

1.1 Enter Site URL

Most users may just enter their base site URL for this field (e.g. example.com). However, if your site meets one of the below cases, please follow these recommendations:

My site uses a subfolder
If your site uses a subfolder, like example.com/blog (where blog is the subfolder), please only enter example.com.

My site uses both www and non-www links
For sites that are accessible from both www & non-www links, such as example.com AND www.example.com, please only enter the one that you wish to send push notifications from.

RECOMMENDED - redirect traffic from one to the other (e.g. users that browse to example.com are redirected to www.example.com), so that all your traffic only goes to one.

1.2 Enter Icon URL

Enter a link to an icon file that is at least 80x80 pixels (RECOMMENDED size is 192x192). The file must be .png, .jpg, or .gif.

2. Upload required files

2.1 Download and unzip the SDK files.

You should have:

manifest.json
OneSignalSDKWorker.js
OneSignalSDKUpdaterWorker.js
2.2 Edit manifest.json:

Change name and short_name to your site's name
Do not change the gcm_sender_id key (482941778795). This is a shared key used for push notifications (previously it required your own key, but this is no longer needed!)
JSON
{ "name": "YOUR_SITE_NAME", "short_name": "YOUR_SITE_NAME", "start_url": "/", "display": "standalone", "gcm_sender_id": "482941778795" }

2.3 Upload the files to the top-level root of your site directory. The following URLs should be publicly accessible:

https://yoursite.com/manifest.json
https://yoursite.com/OneSignalSDKWorker.js
https://yoursite.com/OneSignalSDKUpdaterWorker.js
Once all the steps above have been done install the plugin as any other ImpressPages Plugin

Plugin settings require the App Id and REST API key which can be found as shown below
 
![image](https://cloud.githubusercontent.com/assets/7078331/24985576/5b94e4f2-1fb2-11e7-94df-7e30def2753f.png)

The plugin settings is intuitive
 
![image](https://cloud.githubusercontent.com/assets/7078331/24985581/63e3fff8-1fb2-11e7-8936-d091ef52544f.png)

