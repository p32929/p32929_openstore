---
title: LET - Life Events Tracker
icon: screenshots/let/icon.png
screenshots:
  - screenshots/let/shot-1.png
  - screenshots/let/shot-2.png
  - screenshots/let/shot-3.png
  - screenshots/let/shot-4.png
category: Productivity
kind: personal
summary: Offline habit and life event tracker. Log habits, numbers and notes each day, then see your streaks, patterns and a forecast of the days ahead
tags: [Habit tracker, Life tracker, Daily journal, Mood tracker, Streaks, Offline, Android, Open source]
website: https://github.com/p32929/let
source: https://github.com/p32929/let

platforms:
  Android:
    - version: "1.1.0"
      date: 2026-11-17
      changelog: New Forecast screen that guesses what is likely in the next 14 days from your own patterns, with a reason for each guess
      url: https://github.com/p32929/let/releases/tag/v1.1.0
  Web: https://p32929.github.io/let/
---

> **Still being built.** LET works, but it is a work in progress, so expect rough edges and changes.

LET is a habit and life event tracker for your phone. Most habit apps only ask "did you do it today?". LET lets you log anything about your day, from a simple yes or no to a number or a short note, and then shows you which habits go together on your best days.

I made LET to find patterns. I once heard that history repeats itself, and I think even our own lives follow patterns, so by following them you could predict some things before they happen.

What makes it different: it looks for patterns across everything you track, not just one habit at a time. It can show, for example, which sleep hours or activities often come with a good day. Everything is saved on your phone, works offline, and needs no account.

1. **Track anything:** yes or no events (went outside, exercised), numbers with a unit (hours slept, glasses of water) and text notes (mood, what you ate).
2. **A week view** to fill in each day quickly, and move between weeks with a swipe or a calendar.
3. **Dashboard** with streaks, milestones, personal records and your best days of the week.
4. **Patterns and trends** over 7 days, 30 days, 90 days or a year, with charts.
5. **Forecast** for the next 14 days. LET looks at your history and guesses what is likely on each coming day:
   1. Each day shows the events that are likely, with a % chance. A stronger colour means more likely.
   2. Tap a day to see why, for example "Happened on 8 of the last 10 Mondays".
   3. For numbers and text it also shows the likely value, like "~7 hours".
   4. It uses the day of the week, your recent days (recent days count more), and things that repeat every few days.
   5. A small chart shows the last 14 days next to the next 14.
   6. It needs 14 days of tracking first, and tells you how many more days are needed.
6. **Your own colors** for each event, and you can reorder them.
7. **Export and import** your data as a JSON file, so you can back it up or move phones.
8. **Light and dark mode.** Free and open source.

Great for anyone who wants to understand their days better, not just tick off habits.

To install, open the download page and get the APK for your phone. Most phones need the `arm64-v8a` file, older phones the `armeabi-v7a` one. Open it and allow installs from this source when Android asks. There is also a web version you can open in your browser at https://p32929.github.io/let/.

Want to find the patterns in your own life, your team or your business? Contact me through my portfolio: https://p32929.github.io
