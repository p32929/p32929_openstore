---
title: Manufacturer Battery Optimization
icon: screenshots/manufacturer-battery-optimization/icon.svg
screenshots:
  - screenshots/manufacturer-battery-optimization/v2-1.png
category: Developer Tools
summary: Android helper that sends users to the right battery or autostart setting on Xiaomi, Huawei, Oppo, Vivo, Samsung, OnePlus and other phones
tags: [Android battery optimization, Autostart, Background service, Xiaomi, Huawei, Oppo, Vivo, Kotlin, Java]
website: https://gist.github.com/p32929/41e7af650f6a2c11e9306ab600fb9b03
source: https://gist.github.com/p32929/41e7af650f6a2c11e9306ab600fb9b03

platforms:
  Library: https://gist.github.com/p32929/41e7af650f6a2c11e9306ab600fb9b03
---

Manufacturer Battery Optimization is a single file for Android apps that keep getting stopped in the background. Phones from Xiaomi, Huawei, Honor, Oppo, Realme, OnePlus, Vivo, Samsung, Asus and others add their own battery savers, so alarms, reminders, syncing and background work quietly stop, even when your code is right. This helper shows a short dialog and sends your user to the one right screen to let your app keep running. It was updated in 2026 with a Kotlin version, and the Java version now uses AndroidX.

1. **Opens the right screen:** the phone maker's own autostart or battery screen when the phone has one.
2. **Works on every phone:** if there is no special screen, it opens Android's own battery optimization list.
3. **Knows many phone makers:** Xiaomi, Huawei, Honor, Oppo, Realme, OnePlus, Vivo and iQOO, Samsung, Asus, HTC, LeTV, Transsion and more.
4. **A friendly dialog,** shown once, with a Not now button. Show it again any time from your settings.
5. **Use your own UI if you like:** check `isIgnoringBatteryOptimizations` and call `openSettings` yourself.
6. **Copy and use:** one file in Kotlin or Java, nothing to install.

Great for Android apps with reminders, alarms, wallpapers or background work that must keep running.

To use it, copy `ManufacturerBatteryOptimization.kt` or `ManufacturerBatteryOptimization.java` from the gist into your app, change the package line, and call it from an Activity:

```kotlin
ManufacturerBatteryOptimization.showDialogIfNeeded(this)
```

Want to buy the source code of this app? Contact me through my portfolio: https://p32929.github.io
