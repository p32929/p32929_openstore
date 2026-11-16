---
title: ghcdn
icon: screenshots/ghcdn/icon.png
screenshots:
  - screenshots/ghcdn/1.png
category: Developer Tools
summary: Free GitHub CDN. Turn a GitHub file or Gist link into a link you can use in a script tag, a stylesheet or fetch. A jsDelivr alternative you can host
tags: [GitHub CDN, jsDelivr alternative, Gist, Raw GitHub, CDN, Self-hosted, Developer tools]
website: https://ghcdn.vercel.app/
source: https://github.com/p32929/ghcdn
license: MIT

platforms:
  Web: https://ghcdn.vercel.app/
---

**ghcdn is a free GitHub CDN. Paste a GitHub file or Gist link and get a link you can load in any web page.**

## The problem

You keep a script, a stylesheet or a JSON file in a GitHub repo or a Gist, and you want to use it on a web page. But a browser won't load a file straight from a GitHub page as a script or a stylesheet. Public CDNs like jsDelivr help, but you can't run your own copy of them.

## How ghcdn solves it

Paste the address of a GitHub file or a Gist, press **Generate CDN URL**, and you get a link that works in a `<script>`, a `<link>` or a `fetch()`.

1. **Load JavaScript and CSS** from your own repos on any web page.
2. **Read JSON files** like settings with `fetch()`.
3. **Show a Gist's code** or serve plain text from a repo.
4. **Faster repeat loads,** and you can clear the saved copy when a file changes.
5. **Host it yourself** on Vercel, Netlify, Railway, Docker or most other hosts.

## Who it is for

1. Web developers who keep small scripts and styles on GitHub.
2. Anyone who wants a jsDelivr-style CDN they control.
3. People sharing code snippets from Gists.

## Good to know

It is made for small files like scripts, styles and JSON, not big files or pictures. Add a GitHub token if you need private repositories or a higher request limit.
