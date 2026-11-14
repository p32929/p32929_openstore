---
title: Roxaruu
icon: screenshots/roxaruu/icon.png
screenshots:
  - screenshots/roxaruu/demo.png
video: https://cdn.jsdelivr.net/gh/p32929/p32929_openstore@52364a24b3a0d95c40a747444da39143de50b903/screenshots/roxaruu/demo.mp4
category: Developer Tools
summary: A keyboard-first code editor with terminals built in. Every shortcut is shown where it applies. On macOS, Windows, Linux and any browser
tags: [Code Editor, Terminal, Keyboard Shortcuts, Remote Access, Rust, Claude Code, Developer Tools]
website: https://github.com/p32929/roxaruu
source: https://github.com/p32929/roxaruu
license: MIT

platforms:
  MacOS: https://github.com/p32929/roxaruu#install
  Windows: https://github.com/p32929/roxaruu#install
---

A keyboard-first code editor with terminals built in.

Every action in Roxaruu has a keyboard shortcut, and the shortcuts that work *right where you are* are always on screen. In the editor you see the editor's keys, in a terminal the terminal's, in a list or a dialog its own. You never have to remember a shortcut or dig through a menu to find one.

## Why I made it

I usually work on several projects at the same time, and I start them with a bash script that runs each part in its own terminal. That's where it gets messy: every script opens another terminal *window*. On a big project (say a Flutter app with a few variants, each talking to different backends) I end up with a pile of terminal windows and no idea which is which. Managing them took more effort than the work itself.

I looked for something that already solved this, didn't like what I found, so I made Roxaruu: one window per project, its code and all its terminals together, organised, and everything reachable from the keyboard.

## What it does

**Keyboard first**
- Every action is a named command with a shortcut, and every shortcut can be changed.
- **F1** shows every shortcut. **Ctrl+Shift+P** (**⇧⌘P** on a Mac) finds any command by name.

**Terminals**
- Built in, as tabs, or all of a project's terminals at once in a grid.
- On macOS, a script that opens new Terminal windows opens tabs in Roxaruu instead.
- Each tab says what its program is doing: printing, running, or gone quiet.
- Works with Claude Code and other coding agents: you're told when one has finished or needs you, even when you're looking at something else.

**Editor**
- Syntax highlighting for 23 languages, tabs, split view, find and replace, go to line, go to file, and search across the whole project.
- Opens huge files instantly: it reads only what's on screen.
- Files reopen where you left them, with the cursor and scroll position.

**Remote access**
- Turn it on, set a password, and open the address in any browser, on another computer or a phone. You get the same window, with all its files and terminals.
- Install it on a Linux server (no screen needed) and code on that machine from your browser.

**Make it yours**
- Settings, shortcuts and colour themes are plain JSON files. Four themes are built in, or make your own. Pick a UI font and a code font.
- Also included: a clipboard history, a to-do list, and recent folders.

## Where it stands

Roxaruu works on **macOS, Windows and Linux**, and every feature is meant to work on all three. I use a Mac every day, so that's where it's had the most real use; Windows and Linux are tested, but much less in daily work. It's built with Rust, egui, wgpu and tree-sitter, and it's free and open source (MIT).

I tried to keep it versatile, solid and organised, but I won't pretend it replaces a full IDE. It still has a long way to go. What it does today, it does well, and it gets my work done every day.

For **Linux**, and for how to install on each system, see the [project page](https://github.com/p32929/roxaruu#install).
