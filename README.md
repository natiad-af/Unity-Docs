<img src="https://massets.appsflyer.com/wp-content/uploads/2018/06/20092440/static-ziv_1TP.png"  width="400" >

# appsflyer-unity-plugin

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![GitHub tag](https://img.shields.io/github/v/release/AppsFlyerSDK/appsflyer-unity-plugin)](https://img.shields.io/github/v/release/AppsFlyerSDK/appsflyer-unity-plugin)
[![Unit tests](https://github.com/AppsFlyerSDK/appsflyer-unity-plugin/actions/workflows/main.yml/badge.svg)](https://github.com/AppsFlyerSDK/appsflyer-unity-plugin/actions/workflows/main.yml)


🛠 In order for us to provide optimal support, we would kindly ask you to submit any issues to support@appsflyer.com

> *When submitting an issue please specify your AppsFlyer sign-up (account) email , your app ID , production steps, logs, code snippets and any additional relevant information.*




### <a id="plugin-build-for"> This plugin is built for

- Android AppsFlyer SDK **v6.8.2** 
- iOS AppsFlyer SDK **v6.8.1**

## <a id="breaking-changes">     ❗❗ Breaking changes when updating to 6.6.0 ❗❗
- Starting version 6.6.0, there is no more need to differentiate between iOS and Android APIs. All APIs must be called with `AppsFlyer` class (even if the API is only iOS or Android).

Example:

Before 6.6.0:
```c#
#if UNITY_IOS && !UNITY_EDITOR
    AppsFlyeriOS.waitForATTUserAuthorizationWithTimeoutInterval(60);
#endif
```
---

After 6.6.0:
```c#
#if UNITY_IOS && !UNITY_EDITOR
    AppsFlyer.waitForATTUserAuthorizationWithTimeoutInterval(60);
#endif
```
---

## <a id="breaking-changes">     ❗❗ Breaking changes when updating to 6.3.0 ❗❗

- 6.3.0 supports Universal Windows Platform. As part of this update, the AppsFlyerObjectScript changes to include the app_id for your UWP app. If you made changes to this file, please merge them with the new AppsFlyerObjectScript.
Please also note that you can leave the uwp app id field empty. 

- From version `6.3.0`, we use `xcframework` for iOS platform, then you need to use cocoapods version >= 1.10

## <a id="migration"> ⏩ Migration 
  
Migrating from the old plugin? (version V4) <br/>
View the migration docs [here](/docs/MigrationGuide.md).

⚠️ There are **breaking** changes when migrating to `Unity v5`. This includes new API, different class/package names, and the removal of `com.appsflyer.GetDeepLinkingActivity`.

 ---
## <a id="plugin-build-for"> Plugin
- [Import plugin](/docs/Installation.md)
- [Integrate plugin](/docs/BasicIntegration.md)
- [Test integration](/docs/Testing.md)
- [In-app events](/docs/InAppEvents.md)
- [Uninstall measurement](/docs/UninstallMeasurement.md)
  --
## <a id="plugin-build-for"> Deep Linking
- [integrate](/docs/DeepLinkIntegrate.md)
- [Unified Deep Link (UDL)](/docs/UnifiedDeepLink.md)
- [Direct and deffered Deep Link](/docs/UnifiedDeepLink.md)
- [User invite](/docs/UserInvite.md)
  --
## <a id="plugin-build-for"> API refrence
- [API](/docs/API.md)
    
----  
## [Troubleshooting](/docs/Troubleshooting.md)



