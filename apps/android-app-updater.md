---
title: Android App Updater
icon: screenshots/android-app-updater/icon.svg
screenshots:
  - screenshots/android-app-updater/shot-1.png
category: Developer Tools
summary: Lightweight Android app update checker. Tell users a new version is out, or force them to update, using a JSON file you host
tags: [Android app updater, Update checker, Force update, In-app update, Android library, Java, JitPack, Open source]
website: https://github.com/p32929/AndroidAppUpdater
source: https://github.com/p32929/AndroidAppUpdater

platforms:
  Library: https://github.com/p32929/AndroidAppUpdater
---

Android App Updater is a lightweight update checker for Android apps. Many users never open the Play Store to update, and apps shared outside it have no update system at all. This library reads a small JSON file you host, compares its version code with the installed one, and tells you when a new version is out, so you can ask the user to update.

1. **Host the JSON anywhere:** GitHub, S3, your own server or any web address.
2. **Force an update** when you need to, with one `cancellable` setting in the JSON.
3. **Your own design:** the library gives you the data, and you show your own dialog or message.
4. **Send users anywhere:** the Play Store or a direct download link.
5. **Tiny:** one class, with no Play Services or update SDK needed.

Great for apps shared as APKs outside the Play Store, and for any app that must stop users running an old version.

## Install

Add JitPack to your root `build.gradle`, then the dependency:

```gradle
allprojects { repositories { maven { url 'https://jitpack.io' } } }

dependencies {
    implementation 'com.github.p32929:AndroidAppUpdater:1.0.2'
}
```
