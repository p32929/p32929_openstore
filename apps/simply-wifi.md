---
title: Simply Wifi
icon: screenshots/simply-wifi/icon.png
screenshots:
  - screenshots/simply-wifi/1.png
category: Developer Tools
summary: Control WiFi from a Flutter app in one line. Turn WiFi on or off, list networks, connect, disconnect and forget networks on Android
tags: [Flutter, WiFi, Android, wifi_iot, Dart, Connect to WiFi, pub.dev, Mobile development]
website: https://github.com/p32929/simply_wifi_flutter
source: https://github.com/p32929/simply_wifi_flutter

platforms:
  Library: https://pub.dev/packages/simply_wifi
---

Simply Wifi lets a Flutter app control WiFi with one line per action. The popular wifi_iot package can do a lot, but even simple things like connecting to a network take more code than they should. Simply Wifi wraps it in a few easy calls.

1. **Turn WiFi on or off** from your app.
2. **List the networks around you.**
3. **Connect** by network name, or by its place in the list, with a password if needed.
4. **Disconnect and forget** a saved network.
5. **Asks for the location permission** it needs when you call `init()`.

Great for Flutter apps on Android that need to connect to a WiFi network.

It is an older package, marked as discontinued on pub.dev, and works with apps targeting Android 9 (SDK 28).

## Install

```bash
flutter pub add simply_wifi
```
