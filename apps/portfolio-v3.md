---
title: Fayaz Bin Salam Portfolio v3
icon: screenshots/portfolio-v3/icon.png
screenshots:
  - screenshots/portfolio-v3/shot-1.png
  - screenshots/portfolio-v3/shot-2.png
  - screenshots/portfolio-v3/shot-3.png
category: Developer Tools
summary: Free developer portfolio template with light and dark mode. Change one file to make it yours and publish it on GitHub Pages, no backend needed
tags: [Portfolio template, Developer portfolio, React, TypeScript, shadcn/ui, Tailwind, GitHub Pages, Open source]
website: https://p32929.github.io/
source: https://github.com/p32929/p32929.github.io

platforms:
  Web: https://p32929.github.io/
---

> **The portfolio I use today.** This is the third version of my portfolio and the one running at p32929.github.io right now. [Fayaz Bin Salam Portfolio v2](https://openstore.pfay.workers.dev/app/p32929/portfolio-v2) and [Fayaz Bin Salam Portfolio v1](https://openstore.pfay.workers.dev/app/p32929/portfolio-v1) are the older ones.

Fayaz Bin Salam Portfolio v3 is a free developer portfolio template. Building a personal site from scratch takes days, and keeping it up to date means digging through layout code every time you add a project. Here the site is done: you put your details in one file, and it shows who you are, your skills and all your projects, on desktop, tablet and phone.

What makes it different: every piece of content lives in one file, `src/lib/DynamicValues.ts`. You change data, never the layout. There is no server, and it is free to host on GitHub Pages.

1. **One file to edit:** your details, sections, projects and links are all in `DynamicValues.ts`.
2. **Clean, modern look** built with shadcn/ui and Tailwind, with light and dark mode.
3. **Works on every screen:** desktop, tablet and phone.
4. **Projects grouped by type,** each with an icon, a short line and a link.
5. **Easy to restyle:** colours and design come from `src/index.css`.
6. **Share and support pages** you can link from your READMEs.
7. **Free hosting** on GitHub Pages with two commands.

Great for developers who want a portfolio that is easy to keep up to date.

From my first portfolio on, my goal has been the same: anybody should be able to make their own portfolio without changing much. All three versions are built the same way, with the content kept apart from the layout. In v1 it sits in five small files, in v2 and v3 in a single file. Fork it, put in your own details, and you're done.

How to use it: fork the repository and rename the fork to `your-github-username.github.io`. Clone it, put your own data in `src/lib/DynamicValues.ts`, then run `npm run predeploy` and `npm run deploy`. In the repository settings, under Pages, set the source to the `master` branch.
