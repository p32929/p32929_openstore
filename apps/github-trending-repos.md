---
title: Github Trending Repos
icon: screenshots/github-trending-repos/icon.png
screenshots:
  - screenshots/github-trending-repos/web-1.png
  - screenshots/github-trending-repos/web-2.png
  - screenshots/github-trending-repos/web-3.png
  - screenshots/github-trending-repos/tablet-1.png
  - screenshots/github-trending-repos/tablet-2.png
  - screenshots/github-trending-repos/phone-1.png
  - screenshots/github-trending-repos/phone-2.png
category: Developer Tools
summary: GitHub trending shows one language at a time, so you open a tab for each. This puts 29 languages on one page, sorted by stars, today's stars or forks
tags: [GitHub, Trending, Open Source, Repositories, Developers, Next.js]
website: https://ghtr.fly.dev/
source: https://github.com/p32929/github-trending-repos
license: MIT

platforms:
  Web: https://ghtr.fly.dev/
---

**See what's trending on GitHub in all your languages at once, on one page.**

## The problem

GitHub's own trending page shows one language at a time. If you follow several languages, you have to open a tab for each one and flip between them, and the same repo shows up again and again.

## How it solves it

Open the page and it collects the day's trending repositories for every language at once, with a progress bar while it works, and puts them together in one table.

1. **One table** with the **language**, the **repository** (click to open it on GitHub), its **stars**, the **stars it gained today**, and its **forks**.
2. **No repeats.** Repositories that trend in more than one list are shown once, and the page tells you how many duplicates it removed.
3. **Sort** by **Stars**, **Today** or **Forks**. It starts sorted by what's gaining the most stars today.
4. **Refresh** fetches the latest list, and the page shows when it was last updated.
5. **29 languages,** from Python, JavaScript, TypeScript, Rust and Go to Dart, Kotlin, Swift, Zig and more, plus GitHub's overall trending list.

It's free, needs no sign-up, and works on a phone, a tablet and a computer.

## How it works

GitHub doesn't have a trending API, so a small server reads GitHub's trending pages for each language at the same time, keeps the result in memory, and sends it to your browser. The page is built with Next.js.

Because it reads GitHub's trending pages directly, it will need a fix whenever GitHub changes how that page is built.

It's free and open source (MIT).
