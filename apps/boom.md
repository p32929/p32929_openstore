---
title: Boom
icon: screenshots/boom/icon.png
screenshots:
  - screenshots/boom/shot-1.png
  - screenshots/boom/android-1.png
  - screenshots/boom/android-2.png
  - screenshots/boom/android-3.png
  - screenshots/boom/android-4.png
  - screenshots/boom/android-5.png
  - screenshots/boom/android-6.png
category: Utilities
kind: personal
featured: true
summary: Close all your open apps in one tap. Force quit everything from the Mac menu bar, or close background apps on Android with Shizuku
tags: [Force quit, Quit all apps, Mac menu bar app, macOS, Shut down, Productivity, Swift, Free, Android, Shizuku]
website: https://github.com/p32929/boom
source: https://github.com/p32929/boom
license: MIT

platforms:
  MacOS: https://github.com/p32929/boom/releases/latest
  Android:
    - version: "2.0"
      date: 2026-11-27
      changelog: New Android app with a fresh design, closing apps through Shizuku, with all extra options off by default
      url: https://github.com/p32929/p32929_openstore/releases/tag/boom-android
---

Boom is a tiny Mac menu bar app that force quits all your open apps in one click. When several apps freeze, or you just want a clean slate before a call or the end of the day, you don't have to quit them one by one or wait for each "not responding" window. Click once and they are gone.

What makes it different: most "quit all" tools are a script you have to run, or a menu that also kills parts of macOS. Boom lives in the menu bar and only closes the apps you opened. Finder, the Dock, the menu bar, Control Center, Notification Center, background helpers and Boom itself keep running.

1. **Force Close All:** force quits every app you opened, in one click.
2. **Force Shut Down or Force Restart:** closes every app, then shuts down or restarts your Mac.
3. **Launch at Login,** if you want it there every day.
4. **Stays out of the way:** menu bar only, no Dock icon, and only one copy can run.

Great for anyone whose Mac ends the day with dozens of open apps, or gets stuck with frozen ones.

Boom is inspired by xkill on Linux, where you press a shortcut and click a frozen window to kill it. I wanted something better for my Mac: shutting down or restarting often didn't go through, because a terminal or an iOS simulator wouldn't close. So I made it one click: everything closes, and the Mac shuts down or restarts without me closing things by hand.

**Warning:** Boom closes apps without asking to save, so any unsaved work in them is lost. Save first. Force Shut Down also turns off macOS reopening your windows after a restart, so apps start fresh next time.

## Boom for Android

Boom is on Android too. It closes every app running in the background with one tap, to free memory and save battery. Protect the apps you never want closed with the shield, and everything else goes. It closes apps using Shizuku, which must be installed and running on your phone, and the app shows you how to set it up. All extra options are off by default.

1. **Close every app with one tap,** except the ones you protect, with a confirm step first.
2. **Memory meter** and a list of running, protected and all apps, with search.
3. **Per-app controls:** force stop, protect, and optionally restrict its background or block its wakelocks.
4. **Optional auto-close** a while after the phone locks, with a visible notification.
5. **Home screen shortcut** that closes everything and locks the phone.

On Android, Boom started as a simple app closer using Shizuku. It worked, but it looked ugly, so I gave it a new design.

## Install

Download `Boom-1.2.zip` from the download page, unzip it and move Boom to your Applications folder. The first time, right-click it and choose Open. It needs macOS 13 or newer, and macOS may ask you to allow it to control other apps (System Settings, Privacy & Security, Automation).

On Android, download the APK from the download page and open it to install (arm64-v8a for most phones). Then install Shizuku, start it, and allow Boom in Shizuku.

Want a small Mac tool that saves you a few clicks every day? Contact me through my portfolio: https://p32929.github.io
