---
title: Android App Updater
icon: screenshots/android-app-updater/icon.svg
screenshots:
  - screenshots/android-app-updater/v2-1.png
  - screenshots/android-app-updater/v2-2.png
category: Developer Tools
kind: personal
summary: Android app update checker. Tell users a new version is out, or force them to update, with a ready-made dialog and a JSON file you host
tags: [Android app updater, Update checker, Force update, In-app update, Update dialog, Android library, Kotlin, JitPack]
website: https://github.com/p32929/AndroidAppUpdater
source: https://github.com/p32929/AndroidAppUpdater

platforms:
  Library: https://github.com/p32929/AndroidAppUpdater
---

Android App Updater is a small update checker for Android apps. Many users never open the Play Store to update, and apps shared as APKs have no update system at all. You host one small JSON file anywhere, and the library compares it with the installed version and shows a ready-made update dialog when a newer one is out. It was revamped in 2026: rewritten in Kotlin, with a Material 3 look that follows light and dark mode, and it still works from Java.

I made it to have an easy way to let people know there's an update for my apps.

1. **Built-in update dialog** with the new version and what's new, in your app's colours.
2. **Force an update** when you need to: the dialog then has no Later button.
3. **Host the JSON anywhere:** GitHub, your own server or any web address. No Play Services or update SDK.
4. **Send users anywhere:** the Play Store or a direct download link.
5. **Or build your own UI:** get the parsed data in a callback.
6. **Tiny:** a few small classes, Android 5.0 and newer.

Great for apps shared outside the Play Store, and for any app that must stop users running an old version.

## Install

Add JitPack to your repositories, then the dependency:

```kotlin
// settings.gradle.kts
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()
        maven("https://jitpack.io")
    }
}
```

```kotlin
dependencies {
    implementation("com.github.p32929:AndroidAppUpdater:2.0.0")
}
```

```kotlin
// Shows the dialog only when a newer version is out
AppUpdater.check(this, "https://example.com/update.json")
```

```json
{
  "versionCode": 2,
  "cancellable": true,
  "url": "https://play.google.com/store/apps/details?id=your.app",
  "versionName": "2.0.0",
  "changelog": "1. A fresh new look\n2. Bug fixes"
}
```

The activity that calls it must use an AppCompat or Material theme.

Upgrading from 1.x? The old calls and JSON still work. See "Migrating from 1.x" on the GitHub page.

Want your users to always be on the latest version of your app? Contact me through my portfolio: https://p32929.github.io
