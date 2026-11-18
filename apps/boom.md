---
title: Boom
icon: screenshots/boom/icon.png
screenshots:
  - screenshots/boom/shot-1.png
category: Utilities
kind: personal
featured: true
summary: Force quit every open app on your Mac in one click from the menu bar, or close everything and shut down. Finder and the Dock stay safe
tags: [Force quit, Quit all apps, Mac menu bar app, macOS, Shut down, Productivity, Swift, Free]
website: https://github.com/p32929/boom
source: https://github.com/p32929/boom
license: MIT

platforms:
  MacOS: https://github.com/p32929/boom/releases/latest
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

## Install

Download `Boom-1.2.zip` from the download page, unzip it and move Boom to your Applications folder. The first time, right-click it and choose Open. It needs macOS 13 or newer, and macOS may ask you to allow it to control other apps (System Settings, Privacy & Security, Automation).

Want a small Mac tool that saves you a few clicks every day? Contact me through my portfolio: https://p32929.github.io
