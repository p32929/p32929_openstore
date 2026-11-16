---
title: Put Phone Down
icon: screenshots/put-phone-down/icon.png
screenshots:
  - screenshots/put-phone-down/1.png
  - screenshots/put-phone-down/2.png
  - screenshots/put-phone-down/3.png
  - screenshots/put-phone-down/4.png
  - screenshots/put-phone-down/5.png
  - screenshots/put-phone-down/6.png
  - screenshots/put-phone-down/7.png
category: Productivity
summary: Really put your phone down. Pick a rest time and the app sends you back to rest every time you reach for the phone. Easy one-tap uninstall
tags: [Phone addiction, Digital wellbeing, Focus, Timer, Productivity, Android]

platforms:
  Android:
    - version: "2.0.1"
      date: 2026-11-16
      changelog: New name (was Sleepy - Addiction Controller). Rebuilt in Kotlin and Jetpack Compose with a gentle mode, a one-tap Uninstall button, quiet hours, stats, light and dark mode, no ads
      url: https://github.com/p32929/p32929_openstore/releases/tag/put-phone-down
---

> **An old app, revived.** This app was first made around 2019 and was on Google Play until the account was closed. In 2026 it was rebuilt with modern Android (Kotlin and Jetpack Compose) and a new design, mainly to show it again. Please don't expect it to be actively maintained.

## The story

This was a group project, built with friends. I had a Google Play account, and we published whatever we could build together. Most of my friends hadn't studied computer science; some came from electrical and telecommunication engineering. I was teaching them how to make apps, so we kept each app as simple as possible and as nice as we could, so people would want to download it.

We don't work together any more, but I'm proud of what came out of it. Somehow I made them curious about programming, and after just a few days of building they loved it. Alhamdulillah, many of them still work in software development today, even though they didn't come from that background.

**A phone addiction controller that actually helps you use your phone less.** It used to be called "Sleepy - Addiction Controller".

Many apps only track how much you use your phone. Put Phone Down helps you put it down: you pick a rest time, and until it ends, every time you reach for the phone the app sends you back to rest.

## What it does

1. **Pick a rest time:** 15, 30 or 60 minutes, a custom length, or until a set time.
2. **Two modes:** Gentle shows a calm full-screen "Time to rest" screen and needs no special permission. Lock locks the screen again every time you wake the phone.
3. **Calls still work,** and restarting the phone always ends a session in an emergency.
4. **Daily quiet hours,** a notification when your rest ends, and stats saved on your phone.
5. **Light, dark or system theme.** No ads.

## Easy to uninstall

Lock mode uses Android's Device Administrator permission, and Android blocks uninstalling any app that has it. Earlier versions made people dig through Settings. Now it is one tap:

1. Open the app and tap **Uninstall app** (on the home screen, in Settings or in Help).
2. The app ends any running session, turns off its own lock permission, and opens Android's uninstall screen.
3. Tap **OK**.

You can also just turn the lock permission off with **Turn off** on the home screen. The home screen always shows whether it is on.

## Install

Download the APK and open it. Android will ask you to allow installs from this source. You can turn that permission off again afterwards. If you have the old version installed, uninstall it first (Settings, Security, Device admin apps, Sleepy, Deactivate, then uninstall), because the new one is signed with a different key. Older versions are on the same download page.
