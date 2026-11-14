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
summary: GitHub's daily trending repositories for many languages, all on one page instead of one tab per language. Sort by stars, today's stars or forks
tags: [GitHub, Trending, Open Source, Repositories, Developers, Next.js]
website: https://ghtr.fly.dev/
source: https://github.com/p32929/github-trending-repos
license: MIT

platforms:
  Web: https://ghtr.fly.dev/
---

A simple site that shows GitHub's daily trending repositories for the languages I care about, all on one page instead of one tab per language.

GitHub's own trending page shows one language at a time. If you follow several, that means opening a tab for each and flipping between them. This puts them together in one table: open the page and it collects the day's trending repositories for every language at once, with a progress bar while it works.

## What you see

- One table with the **language**, the **repository** (click to open it on GitHub), its **stars**, the **stars it gained today**, and its **forks**.
- Repositories that trend in more than one list are shown once, and the page tells you how many duplicates it removed.
- Click **Stars**, **Today** or **Forks** to sort. It starts sorted by what's gaining the most stars today.
- A **Refresh** button fetches the latest list, and the page shows when it was last updated.
- It covers 29 languages, from Python, JavaScript, TypeScript, Rust and Go to Dart, Kotlin, Swift, Zig and more, plus GitHub's overall trending list.

It's free, needs no sign-up, and works on a phone, a tablet and a computer.

## How it works

GitHub doesn't have a trending API, so a small server reads GitHub's trending pages for each language at the same time, keeps the result in memory, and sends it to your browser. The page is built with Next.js.

Because it reads GitHub's trending pages directly, it will need a fix whenever GitHub changes how that page is built.

It's free and open source (MIT).
