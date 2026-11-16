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
summary: Can't stop picking up your phone? Set a time and the phone stays locked until it is over. Every time you reach for it, it locks again
tags: [Phone addiction, Digital wellbeing, Focus, Timer, Productivity, Android]

platforms:
  Android:
    - version: "2.0.1"
      date: 2026-11-16
      changelog: New name (was Sleepy - Addiction Controller). Rebuilt in Kotlin and Jetpack Compose with a gentle mode, a one-tap Uninstall button, quiet hours, stats, light and dark mode, no ads
      url: https://github.com/p32929/p32929_openstore/releases/tag/put-phone-down
---

> **An old app, revived.** This app was first made around 2019 and was on Google Play until the account was closed. In 2026 it was rebuilt with modern Android (Kotlin and Jetpack Compose) and a new design, mainly to show it again. Please don't expect it to be actively maintained.

**Can't stop picking up your phone? This app locks it for you until your break is over.**

## The problem

You put the phone down to sleep, study or work, and a minute later it is back in your hand. Willpower alone does not work, and most "digital wellbeing" apps only count your screen time. They tell you there is a problem, but they do nothing to stop you.

## How Put Phone Down solves it

You choose how long you want to stay off your phone, for example 30 minutes. Until that time is over, the phone is locked. Every time you pick it up and try to use it, the app locks the screen again and sends you back to rest. You can't cheat by just opening the phone.

1. **Set a time:** 15, 30 or 60 minutes, any custom length, or until a set clock time.
2. **Lock mode** locks the screen again every time you wake the phone, until the time is up.
3. **Gentle mode** shows a full-screen "Time to rest" screen instead, for people who want a softer nudge. It needs no special permission.
4. **Daily quiet hours** start a rest by themselves at the same time every day, for example at bedtime.
5. **Calls still work,** and restarting the phone always ends a rest in an emergency.
6. **Stats** show how long you rested and how many times you reached for the phone. They stay on your phone.
7. **Light, dark or system theme.** No ads. It used to be called "Sleepy - Addiction Controller".

## Easy to uninstall

Lock mode uses Android's Device Administrator permission, and Android blocks uninstalling any app that has it. Earlier versions made people dig through Settings. Now it is one tap:

1. Open the app and tap **Uninstall app** (on the home screen, in Settings or in Help).
2. The app ends any running session, turns off its own lock permission, and opens Android's uninstall screen.
3. Tap **OK**.

You can also just turn the lock permission off with **Turn off** on the home screen. The home screen always shows whether it is on.

## The story

This was a group project, built with friends. I had a Google Play account, and we published whatever we could build together. Most of my friends hadn't studied computer science; some came from electrical and telecommunication engineering. I was teaching them how to make apps, so we kept each app as simple as possible and as nice as we could, so people would want to download it.

We don't work together any more, but I'm proud of what came out of it. Somehow I made them curious about programming, and after just a few days of building they loved it. Alhamdulillah, many of them still work in software development today, even though they didn't come from that background.

## Install

Download the APK and open it. Android will ask you to allow installs from this source. You can turn that permission off again afterwards. If you have the old version installed, uninstall it first (Settings, Security, Device admin apps, Sleepy, Deactivate, then uninstall), because the new one is signed with a different key. Older versions are on the same download page.
