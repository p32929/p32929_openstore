---
title: ByteBroom
icon: screenshots/bytebroom/icon.png
screenshots:
  - screenshots/bytebroom/1.png
  - screenshots/bytebroom/2.png
category: Utilities
summary: Finds what is safe to delete on your Mac, like build folders, caches and leftover app files, sorted by size with a reason for each
tags: [macOS, Disk cleaner, Developer tools, Cache cleaner, node_modules, Xcode, Rust, Open source]
website: https://github.com/p32929/bytebroom
source: https://github.com/p32929/bytebroom

platforms:
  MacOS: https://github.com/p32929/bytebroom/releases/latest
---

**Find what is safe to delete on your Mac, and free the space.**

ByteBroom scans your whole disk and lists everything over 50 MB that it knows how to judge, sorted by size. Every item says why it is there, so you decide with the facts in front of you.

## What it does

1. **Safe to delete.** Things that come back by themselves, or with a rebuild or reinstall: project build folders (`node_modules`, `target`, `build`, `.dart_tool`, `Pods`, `.venv` and more, for many languages), package manager caches (npm, Yarn, pnpm, Cargo, Gradle, pip and others), Xcode build data, and app caches and logs.
2. **Look first.** Things where you lose what is inside, so you should check before deleting: the Trash, iOS simulators, Android emulators, Docker and VM data, Downloads, temporary files, and backups.
3. **Apps.** Every installed app with the files it has spread around your system. Tick the box next to an app to remove it completely.
4. **Move to Trash or delete for good.** Trash can be undone. Permanent delete frees the space right away, with a progress window.
5. **Light, dark or system theme.**

## Built to not delete the wrong thing

1. A folder that git tracks is never offered. A `build` folder with committed files in it is source, not junk.
2. Projects need proof. A `target` folder only counts if a `Cargo.toml` sits next to it, and `node_modules` needs a `package.json`.
3. Your home folder, anything above it, and system folders such as `/Library/Caches` itself are off limits.
4. Links are removed, never followed, so deleting a link leaves what it points to.

## Install

Download the `.dmg` from the latest release, open it and drag ByteBroom onto Applications. Releases are built for Apple Silicon Macs. On an Intel Mac, build it from source with Rust.

The app is not notarized by Apple yet, so the first time macOS asks you to allow it: open System Settings, Privacy & Security, and click Open Anyway. For the best results, also add ByteBroom under Full Disk Access, or macOS hides some folders from it.
