---
title: str_template
icon: screenshots/str-template/icon.png
screenshots:
  - screenshots/str-template/shot-1.png
category: Developer Tools
kind: personal
summary: Tiny string templating library for JavaScript and TypeScript. Fill placeholders like {name} in a string from an object, in Node or the browser
tags: [String template, Templating, String format, TypeScript, JavaScript, Node.js, Browser, npm]
website: https://github.com/p32929/str_template
source: https://github.com/p32929/str_template

platforms:
  Library: https://www.npmjs.com/package/str-template-ts
---

str_template is a tiny string templating library for JavaScript and TypeScript. When a message or text comes from a file, a database or a translation, you can't use a template literal, and joining strings by hand gets ugly. Write `{placeholders}` in the string and fill them from an object with one call.

I made it because I needed a small string templating tool. The others out there pretty much all do the same thing, so I thought: okay, let's make my own as well.

1. **One function:** `StrTemplate.format(text, values)`.
2. **Your own separator:** use `{}` by default, or something like `[[ ]]` if braces are already in your text.
3. **Works the same in Node.js and the browser.**
4. **Written in TypeScript,** small and fast.

Great for message templates, emails and any text with values filled in later.

## Install

```bash
npm install str-template-ts
```

It uses `String.replaceAll`, so it needs Node 15 or newer, or a modern browser.

```ts
StrTemplate.format('Hello {name}!', { name: 'Fayaz' }) // Hello Fayaz!
```

Want help tidying up how your app handles text and messages? Contact me through my portfolio: https://p32929.github.io
