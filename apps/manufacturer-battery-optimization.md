---
title: Manufacturer Battery Optimization
icon: screenshots/manufacturer-battery-optimization/icon.svg
screenshots:
  - screenshots/manufacturer-battery-optimization/1.png
category: Developer Tools
summary: Android helper class that sends users to the right battery or autostart setting on Xiaomi, Huawei, Oppo, Vivo, Samsung and other phones
tags: [Android battery optimization, Autostart, Background service, Xiaomi, Huawei, Oppo, Vivo, Android, Java]
website: https://gist.github.com/p32929/41e7af650f6a2c11e9306ab600fb9b03
source: https://gist.github.com/p32929/41e7af650f6a2c11e9306ab600fb9b03

platforms:
  Library: https://gist.github.com/p32929/41e7af650f6a2c11e9306ab600fb9b03
---

Manufacturer Battery Optimization is a single Java class for Android apps that keep getting stopped in the background. Many phone makers add their own battery savers, so alarms, reminders and services stop working on some phones even when your code is right. This class shows your users a dialog and takes them straight to the setting on their phone where they can let your app run.

1. **Knows the special settings screens** of Asus, ColorOS and Oppo, Huawei, Xiaomi (MIUI), Samsung, Vivo and iQOO, HTC, LeTV, Transsion and more.
2. **One call:** `ManufacturerBatteryOptimization.showAddToWhitelistDialog(context)`.
3. **Only where it helps:** it shows the dialog only when the phone has one of these screens.
4. **Copy and use:** one file, nothing to install.

Great for Android apps with reminders, alarms, wallpapers or background work that must keep running.

To use it, copy `ManufacturerBatteryOptimization.java` from the gist into your project and change the package name.
