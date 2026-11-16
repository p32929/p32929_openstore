---
title: ByteBroom
icon: screenshots/bytebroom/icon.png
screenshots:
  - screenshots/bytebroom/1.png
  - screenshots/bytebroom/2.png
category: Utilities
summary: Mac disk cleaner that finds what is safe to delete, like old build folders, caches and leftover app files, and frees up space in a few clicks
tags: [Mac disk cleaner, Free up space, macOS, Cache cleaner, App uninstaller, node_modules, Xcode, Developer tools]
website: https://github.com/p32929/bytebroom
source: https://github.com/p32929/bytebroom

platforms:
  MacOS: https://github.com/p32929/bytebroom/releases/latest
---

ByteBroom is a free Mac disk cleaner for when your Mac says "Your disk is almost full" and you have no idea what is taking the space. Most of it hides where you never look: old `node_modules` and build folders, caches, Xcode data, simulators, and files left behind by apps you removed long ago. ByteBroom finds all of it, tells you what each item is, and shows what is safe to delete so you can free up space in a few clicks.

It scans your whole disk and lists everything over 50 MB, biggest first, with a note on whether each item comes back by itself.

1. **Safe to delete:** project build folders (`node_modules`, `target`, `build`, `Pods`, `.venv` and more), package manager caches (npm, Yarn, pnpm, Cargo, Gradle, pip and others), Xcode build data, and app caches and logs.
2. **Look first:** the Trash, iOS simulators, Android emulators, Docker and VM data, Downloads, temporary files and backups are marked so you check before deleting.
3. **Remove apps completely,** with every file they spread around your Mac, in one tick.
4. **Undo if you need to:** move things to the Trash, or delete them for good to get the space back right away.
5. **Your work is safe:** folders tracked by git, your home folder and system folders are never offered.
6. **Light and dark mode.**

Great for developers whose Mac keeps filling up, and for anyone who wants to remove apps without leaving files behind.

Download the `.dmg`, open it and drag ByteBroom onto Applications. It works on Apple Silicon Macs. The first time, macOS may block it: open System Settings, Privacy & Security, and click Open Anyway. Give it Full Disk Access so it can find every folder.
