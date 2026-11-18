---
title: ghcdn
icon: screenshots/ghcdn/icon.png
screenshots:
  - screenshots/ghcdn/1.png
category: Developer Tools
kind: personal
summary: Free GitHub CDN. Turn a GitHub file or Gist link into a link you can use in a script tag, a stylesheet or fetch. A jsDelivr alternative you can host
tags: [GitHub CDN, jsDelivr alternative, Gist, Raw GitHub, CDN, Self-hosted, Developer tools]
website: https://ghcdn.vercel.app/
source: https://github.com/p32929/ghcdn
license: MIT

platforms:
  Web: https://ghcdn.vercel.app/
---

ghcdn is a free GitHub CDN. You keep a script, a stylesheet or a JSON file on GitHub and want to use it on a web page, but a browser won't load a file straight from a GitHub page. Paste the address of a GitHub file or a Gist, press **Generate CDN URL**, and you get a link that works in a `<script>`, a `<link>` or a `fetch()`. It works like jsDelivr, except you can run your own copy.

1. **Load JavaScript and CSS** from your own repos on any web page.
2. **Read JSON files** like settings with `fetch()`.
3. **Show a Gist's code** or serve plain text from a repo.
4. **Faster repeat loads,** a list of the files it has cached, and you can clear the saved copy when a file changes.

I made ghcdn because loading files from GitHub into my web pages kept running into CORS errors. Some tools fixed part of it, but none handled both GitHub files and Gists for free, so I built my own. Now I can put any file on my pages, and it shows me which files are cached.

It is made for small files like scripts, styles and JSON, not big files or pictures.

## Host it yourself

Deploy it to Vercel, Netlify, Railway, Docker or most other hosts. Add a GitHub token if you need private repositories or a higher request limit.

Want your files served to your web pages without the CORS trouble? Contact me through my portfolio: https://p32929.github.io
