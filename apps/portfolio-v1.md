---
title: Portfolio v1
icon: screenshots/portfolio-v1/icon.png
screenshots:
  - screenshots/portfolio-v1/shot-1.png
  - screenshots/portfolio-v1/shot-2.png
category: Developer Tools
summary: My very first React project, a simple developer portfolio template from 2018. Kept as history. Edit five small files and publish it on GitHub Pages
tags: [Portfolio template, Developer portfolio, Personal website, React, Material UI, GitHub Pages, Open source]
website: https://p32929.github.io/portfolio-v1/
source: https://github.com/p32929/portfolio-v1

platforms:
  Web: https://p32929.github.io/portfolio-v1/
---

> **My very first React project.** I made this in 2018 while I was just starting to learn React and trying things out. It looks a bit ugly today, but back then it looked okay to me for some reason :D I keep it as a piece of history, to remember how far I have come. [Portfolio v2](https://openstore.pfay.workers.dev/app/p32929/portfolio-v2) is the newer and much nicer one.

Portfolio v1 is a free single-page developer portfolio template made with React and Material UI. Making a portfolio site from scratch takes days of design and layout work. Here the layout is done: you fill in your own text and links, and it is ready to put online.

What makes it different: all the content lives in five small plain JavaScript files, one per section, so you change text, not code. There is no server, and it deploys to GitHub Pages for free with one command.

1. **Ready-made sections:** Home, Skills, Projects and Contact, with a side menu.
2. **Edit text, not code:** each section reads from its own file in `src/vars/`.
3. **Project cards** with an icon, a short line and a link for each app.
4. **Free hosting:** `npm run deploy` puts it on GitHub Pages.
5. **Free and open source** (MIT).

Great for developers who want a simple portfolio online in about ten minutes.

How to use it: fork the repository and clone your fork, then run `npm install`. Edit the files in `src/vars/` (home, skills, projects, contact and the side menu). Set `homepage` in `package.json` to your own address, run `npm run deploy`, and set GitHub Pages to the `gh-pages` branch in your repository settings.
