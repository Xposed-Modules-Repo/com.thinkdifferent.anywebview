# AnyWebView

Any WebView is OK!

![preview](https://raw.githubusercontent.com/neoblackxt/AnyWebView/master/.github/webviews.jpg)

Android Framework should be selected in LSPosed.

A webview app must be installed for all users (or in all spaces) to be selectable. Maybe deleting redundant users is alternative.
adb command:

Get USER_ID list:

`adb shell pm list users`

Each user entry is as follow: UserInfo{USER_ID:USERNAME:INT} , USER_ID 0 is the main user.

Install apk for specific USER_ID:

`adb install --user USER_ID PATH_TO_APK`

Delete a user (be careful, you may lose important data):

`adb shell pm remove-user USER_ID`

Reboot to take effect.
