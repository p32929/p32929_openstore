---
title: Remote for Claude Code
icon: screenshots/remote-for-claude-code/icon.png
screenshots:
  - screenshots/remote-for-claude-code/1.png
  - screenshots/remote-for-claude-code/2.png
  - screenshots/remote-for-claude-code/3.png
  - screenshots/remote-for-claude-code/4.png
  - screenshots/remote-for-claude-code/5.png
category: Developer Tools
kind: personal
featured: true
summary: Control Claude Code on your computer from your Android phone. Start sessions, chat and answer permission prompts, paired with a simple desktop app
tags: [Claude Code, Remote control, AI coding, Mobile coding, Claude, Developer tools, QR pairing, Desktop app, Linux]

platforms:
  Android:
    - version: "2.0.0"
      date: 2026-11-27
      changelog: New name, a desktop app for the server (no terminal or scripts), and a version check between phone and computer
      url: https://github.com/p32929/p32929_openstore/releases/tag/remote-for-claude-code
  MacOS:
    - version: "2.0.0"
      date: 2026-11-27
      changelog: New desktop app to run the server, with a pairing QR code, status and log
      url: https://github.com/p32929/p32929_openstore/releases/tag/remote-for-claude-code
  Windows:
    - version: "2.0.0"
      date: 2026-11-27
      changelog: New desktop app to run the server, with a pairing QR code, status and log
      url: https://github.com/p32929/p32929_openstore/releases/tag/remote-for-claude-code
  Linux:
    - version: "2.0.0"
      date: 2026-11-27
      changelog: New desktop app to run the server, with a pairing QR code, status and log
      url: https://github.com/p32929/p32929_openstore/releases/tag/remote-for-claude-code
---

Remote for Claude Code lets you use Claude Code on your computer from your Android phone, so you can keep a coding session going, answer its questions and approve its actions when you are away from your desk. Browse your project folders, start or resume sessions and chat with Claude Code, right from your phone.

What makes it different: there is nothing to set up by hand. The computer side is a normal desktop app. Install it, press Start server and scan the QR code with the phone app. No terminal, no Node.js install, no scripts.

1. **Pair with a QR code,** or type the address and password yourself.
2. **Your projects and sessions:** browse folders, start a new session or resume an earlier one.
3. **Chat with Claude Code** from your phone, and answer its permission prompts.
4. **Notifications** when Claude Code needs you.
5. **Desktop app** with the server status, the pairing QR code and address, a log, Start and Stop, the port, and an optional Start at login (off by default).
6. **Claude Code check:** the desktop app tells you if Claude Code is ready, not installed, or installed but not signed in, and how to fix it.
7. **Version check:** the phone app warns you if the desktop app and the phone app don't match, and tells you which one to update.
8. **Works in a browser too:** scan the QR code with any phone camera to use it from the browser.

I made it because I wanted to control Claude Code from my phone. Then I wanted others to be able to use it too, so I made the server a desktop app, easy to install with no setup.

Good to know: install the desktop app on your computer (Mac, Windows or Linux). The Claude Code CLI must be installed and signed in on that computer, because your sessions run there with your own Claude Code account. The phone and the computer must be on the same Wi-Fi, and the phone app and desktop app versions must match (both 2.0.0). Closing the desktop app's window stops the server. Remote for Claude Code is not made by Anthropic.

## Install

On your phone, download the APK from the download page and open it to install (arm64-v8a for most phones). On your computer, download the desktop app from the same page: the `.dmg` for a Mac with Apple Silicon, the `.exe` for Windows, or the `.AppImage` for Linux. Open it, press Start server, then scan the QR code with the phone app.

Want your own tools reachable from your phone? Contact me through my portfolio: https://p32929.github.io
