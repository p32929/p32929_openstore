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

**ByteBroom is a free Mac disk cleaner that shows you what is safe to delete and frees up space in a few clicks.**

## The problem

Your Mac says "Your disk is almost full". Most of that space is hidden in places you never look: old `node_modules` and build folders, caches, Xcode data, simulators, and files left behind by apps you already removed. Finding them by hand takes hours, and deleting the wrong folder can break a project or lose your work.

## How ByteBroom solves it

ByteBroom scans your whole disk and lists everything over 50 MB, biggest first. Each item says what it is and whether it comes back by itself, so you know what you can delete without worry.

1. **Safe to delete:** project build folders (`node_modules`, `target`, `build`, `Pods`, `.venv` and more), package manager caches (npm, Yarn, pnpm, Cargo, Gradle, pip and others), Xcode build data, and app caches and logs.
2. **Look first:** the Trash, iOS simulators, Android emulators, Docker and VM data, Downloads, temporary files and backups, marked so you check before deleting.
3. **Remove apps completely:** every installed app with all the files it spread around your Mac, removed in one tick.
4. **Undo if you need to:** move things to the Trash, or delete them for good to free the space right away.
5. **It won't touch your work:** folders tracked by git, your home folder and system folders are never offered.
6. **Light and dark mode.**

## Who it is for

1. Developers whose Mac fills up with build folders and caches.
2. Anyone who sees "disk almost full" and doesn't know what to delete.
3. People who want to remove apps without leaving files behind.

## Install

Download the `.dmg`, open it and drag ByteBroom onto Applications. It works on Apple Silicon Macs. The first time, macOS may block it: open System Settings, Privacy & Security, and click Open Anyway. Give it Full Disk Access so it can find every folder.
