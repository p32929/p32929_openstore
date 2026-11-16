---
title: ghcdn
icon: screenshots/ghcdn/icon.png
screenshots:
  - screenshots/ghcdn/1.png
category: Developer Tools
summary: Browsers won't run a script or stylesheet straight from a GitHub link. Paste the file or Gist link and get a CDN link that works. Host it yourself
tags: [CDN, GitHub, Gist, Self-hosted, jsDelivr Alternative, Next.js, Developer Tools]
website: https://ghcdn.vercel.app/
source: https://github.com/p32929/ghcdn
license: MIT

platforms:
  Web: https://ghcdn.vercel.app/
---

**Your file is on GitHub, but your web page can't load it. ghcdn gives you a link that works.**

## The problem

You keep a script, a stylesheet or a JSON file in a GitHub repo or a Gist, and you want to use it on a web page. But GitHub shows files on its own pages, and a browser won't run those as a script or a stylesheet. Public CDNs like jsDelivr help, but you can't run your own copy of them.

## How ghcdn solves it

Paste the address of a file in a GitHub repository, or of a Gist, press **Generate CDN URL**, and you get a link that works in a `<script>`, a `<link>` or a `fetch()`. You can host ghcdn yourself.

## How to use it

1. Paste a GitHub file address (like `https://github.com/username/repo/blob/branch/path/file.js`) or a Gist address.
2. Press **Generate CDN URL**.
3. Copy the link and drop it into your page.

It's useful for things like:

1. Loading a JavaScript file or a CSS stylesheet from one of your repos.
2. Reading a JSON settings file with `fetch()`.
3. Showing a Gist's code on a page.
4. Serving plain text or documentation from a repo.

## What it does for you

1. Serves files from GitHub repositories and Gists through a normal web link.
2. Keeps recently used files in memory, so repeat requests are faster.
3. Lets you clear (purge) the saved copy when a file changes.

## Host it yourself

It's the same idea as jsDelivr, but you can run your own copy. It's a small Next.js app: deploy it to Vercel, Netlify, Railway, Docker or most other hosts. You can add a GitHub token (optional) for a higher request limit.

## Good to know

1. It isn't made for large files, apps or pictures. Use a proper image host for those.
2. Without a GitHub token, it's limited by GitHub's request limits.
3. Private repositories aren't supported unless you give it a token.
4. If a file changes often, you may need to purge the saved copy.

It's free and open source (MIT).
