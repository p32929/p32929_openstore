---
title: FCloud
icon: screenshots/fcloud/icon.png
screenshots:
  - screenshots/fcloud/1.png
  - screenshots/fcloud/2.png
  - screenshots/fcloud/3.png
  - screenshots/fcloud/4.png
  - screenshots/fcloud/5.png
category: Tools
kind: personal
featured: true
summary: Back up and restore your contacts, call logs and SMS with your Google account. Free, simple, and no duplicates when you restore on a new phone
tags: [Contacts backup, SMS backup, Call log backup, Restore contacts, Backup and restore, New phone, Google sign-in, Firebase, Free]

platforms:
  Android:
    - version: "2.0"
      date: 2026-11-27
      changelog: Rebuilt from scratch with a new design, Google sign-in, a working contacts restore and no duplicates
      url: https://github.com/p32929/p32929_openstore/releases/tag/fcloud
---

FCloud is a free app to back up and restore your contacts, call logs and text messages (SMS), so you get them back after you reset your phone or move to a new one. Sign in with Google, choose what to back up, and press Back up now. On the new phone, sign in again, pick a backup and restore it.

What makes it different: it does only the small text things you need again, and it keeps it as easy as possible. Restoring never doubles anything: whatever is already on the phone is skipped. Nothing is chosen or uploaded until you say so.

1. **Back up contacts, call logs and SMS,** each one chosen separately. Contacts keep their names, numbers, emails, addresses, notes and photos.
2. **See what you have:** it shows how many contacts, calls and messages are on the phone.
3. **Your backups in one list,** with the date, phone, size and counts.
4. **Restore all or only some parts** of a backup, with no duplicates.
5. **Delete a backup** whenever you want.
6. **Light and dark theme,** with your wallpaper colours on Android 12 and newer.

I made it because I wanted an easy way to back up and restore contacts, messages and call logs, the small text things people need again after resetting a phone. No photos, just the text data, as easy as possible, and completely free.

Good to know: your backups are stored in your own private space on Firebase (Google Cloud), linked to your Google account, and only your signed-in account can read them. They are protected in transit and at rest by Google, but they are not end-to-end encrypted, and the app shows you this before every upload. To restore SMS, Android only lets the default SMS app write messages, so FCloud asks to be your default SMS app for a moment, then takes you to the setting to switch back to your usual app.

## Install

Download the APK from the download page and open it to install (arm64-v8a for most phones).

Need your phone's data backed up in a simple way? Contact me through my portfolio: https://p32929.github.io
