---
title: AndroidAppLockscreen
icon: screenshots/androidapplockscreen/icon.svg
screenshots:
  - screenshots/androidapplockscreen/v2-1.png
  - screenshots/androidapplockscreen/v2-2.png
  - screenshots/androidapplockscreen/v2-3.png
category: Developer Tools
kind: personal
summary: Android app lock screen library. Add a 4 to 8 digit passcode lock to your app in a few lines, with fingerprint unlock and light and dark mode
tags: [Android lock screen, App lock, PIN lock, Passcode, Fingerprint unlock, Android library, Kotlin, JitPack]
website: https://github.com/p32929/AndroidAppLockscreen
source: https://github.com/p32929/AndroidAppLockscreen

platforms:
  Library: https://github.com/p32929/AndroidAppLockscreen
---

AndroidAppLockscreen adds a passcode lock screen to your Android app. Building one yourself means designing a keypad, storing the passcode safely and locking again whenever people come back to the app. With this library it takes a few lines: your app asks for a 4 to 8 digit passcode when it opens and every time someone returns to it. It was revamped in 2026: rewritten in Kotlin, with a Material 3 look that follows light and dark mode, and it still works from Java.

I made it so I could use it in all my apps: an easy way to add password protection to every Android app I make.

1. **A clean lock screen** with round number keys, dots that fill in as you type, a shake and a small vibration on a wrong passcode.
2. **Set, change or turn off** the passcode with one call each.
3. **Fingerprint or face unlock,** turned on with one line.
4. **Locks again** when people leave the app and come back.
5. **Passcodes are stored as a salted hash,** not as plain text.
6. **Your own look if you want it:** pass your own theme or background colour. On Android 12 and newer it uses the phone's own colours.
7. **"Forgot passcode?"** button that runs your own code.

Great for diary, notes, finance or any app that should ask for a passcode before it opens.

## Install

It works on Android 5.0 (API 21) and newer, from Kotlin or Java.

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
    implementation("com.github.p32929:AndroidAppLockscreen:2.0.0")
}
```

```kotlin
class MainActivity : LockscreenHandler() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
        if (savedInstanceState == null) EasyLock.checkPassword(this)
    }
}

EasyLock.setPassword(this)          // set a passcode
EasyLock.setBiometricEnabled(true)  // allow fingerprint unlock
```

Upgrading from 1.x? Your old calls keep working and saved passcodes still unlock. See "Migrating from 1.x" on the GitHub page.

Want a lock screen that matches your app's look? Contact me through my portfolio: https://p32929.github.io
