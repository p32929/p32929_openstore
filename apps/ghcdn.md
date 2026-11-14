---
title: ghcdn
icon: screenshots/ghcdn/icon.png
screenshots:
  - screenshots/ghcdn/1.png
category: Developer Tools
summary: Paste a GitHub file or Gist link and get a CDN link for a script, a stylesheet or fetch(). A jsDelivr-style tool you can host yourself
tags: [CDN, GitHub, Gist, Self-hosted, jsDelivr Alternative, Next.js, Developer Tools]
website: https://ghcdn.vercel.app/
source: https://github.com/p32929/ghcdn
license: MIT

platforms:
  Web: https://ghcdn.vercel.app/
---

**Turn a GitHub file or a Gist into a link you can use straight in your web page.**

GitHub shows your files on its own pages, which a browser won't run as a script or a stylesheet. ghcdn fixes that. Paste the address of a file in a GitHub repository, or of a Gist, press **Generate CDN URL**, and you get a link that works in a `<script>`, a `<link>` or a `fetch()`.

## How to use it

1. Paste a GitHub file address (like `https://github.com/username/repo/blob/branch/path/file.js`) or a Gist address.
2. Press **Generate CDN URL**.
3. Copy the link and drop it into your page.

It's useful for things like:
- loading a JavaScript file or a CSS stylesheet from one of your repos,
- reading a JSON settings file with `fetch()`,
- showing a Gist's code on a page,
- serving plain text or documentation from a repo.

## What it does for you

- Serves files from GitHub repositories and Gists through a normal web link.
- Keeps recently used files in memory, so repeat requests are faster.
- Lets you clear (purge) the saved copy when a file changes.

## Host it yourself

It's the same idea as jsDelivr, but you can run your own copy. It's a small Next.js app: deploy it to Vercel, Netlify, Railway, Docker or most other hosts. You can add a GitHub token (optional) for a higher request limit.

## Good to know

- It isn't made for large files, apps or pictures. Use a proper image host for those.
- Without a GitHub token, it's limited by GitHub's request limits.
- Private repositories aren't supported unless you give it a token.
- If a file changes often, you may need to purge the saved copy.

It's free and open source (MIT).
