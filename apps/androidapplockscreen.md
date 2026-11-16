---
title: AndroidAppLockscreen
icon: screenshots/androidapplockscreen/icon.svg
screenshots:
  - screenshots/androidapplockscreen/shot-1.png
  - screenshots/androidapplockscreen/shot-2.png
category: Developer Tools
summary: Android app lock screen library. Add a clean PIN lock to your app in two steps, with set, change and disable password built in
tags: [Android lock screen, App lock, PIN lock, Passcode, Android library, Java, JitPack, Open source]
website: https://github.com/p32929/AndroidAppLockscreen
source: https://github.com/p32929/AndroidAppLockscreen

platforms:
  Library: https://github.com/p32929/AndroidAppLockscreen
---

AndroidAppLockscreen is a small Android library that adds a PIN lock screen to your app. Building a passcode screen yourself means designing the keypad, saving the password and handling every screen of your app. With this library it takes two steps, and you get a clean, minimal lock screen inspired by the Diaro diary app.

1. **Two-step setup:** extend your activities from `LockscreenHandler` and call `EasyLock.checkPassword(this)`.
2. **Set, change or turn off** the password with one call each.
3. **"Forgot password"** taps go to your own handler.
4. **Your own colours:** set the lock screen background colour.

Great for diary, notes, finance or any Android app that should ask for a PIN before it opens.

## Install

Add JitPack to your root `build.gradle`, then the dependency:

```gradle
allprojects { repositories { maven { url 'https://jitpack.io' } } }

dependencies {
    implementation 'com.github.p32929:AndroidAppLockscreen:1.2'
}
```
