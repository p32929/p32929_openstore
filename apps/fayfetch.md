---
title: fayfetch
icon: screenshots/fayfetch/icon.png
screenshots:
  - screenshots/fayfetch/shot-1.png
category: Developer Tools
summary: Simple fetch wrapper for JavaScript and Node.js. Make GET, POST, PUT, DELETE and file upload calls in one line with params and headers
tags: [Fetch wrapper, HTTP client, REST API, JavaScript, Node.js, TypeScript, npm, Developer tools]
website: https://github.com/p32929/FayFetch
source: https://github.com/p32929/FayFetch

platforms:
  Library: https://www.npmjs.com/package/fayfetch
---

fayfetch is a simple wrapper around fetch for JavaScript and Node.js. Calling a REST API with plain fetch means building the query string, setting headers, turning the body into JSON and checking the response every time. fayfetch does that for you: pass the URL, params, headers and body, and get the status and the JSON back in one callback.

I made it back when I didn't know much JavaScript yet, and TypeScript even less. I wanted a quick, hacky way to make fetch calls as easy as possible for me. I know it's not the best way to do it, but I gave it a try.

1. **One line per request:** `get`, `post`, `put` and `deletee` with params, headers and a body.
2. **File uploads:** upload a file, or send your own `FormData`.
3. **One simple callback:** you get the status code, the JSON data and whether it worked.
4. **Works with `require` or `import`.**

Great for small Node.js scripts and apps that talk to a REST API.

## Install

```bash
npm install fayfetch
```

```js
import { FayFetch } from 'fayfetch'

FayFetch.get(url, params, headers, (status, jsonData, ok) => {
  if (ok) console.log(jsonData)
})
```

Want a clean API layer for your JavaScript project? Contact me through my portfolio: https://p32929.github.io
