---
title: fjsondb
icon: screenshots/fjsondb/icon.png
screenshots:
  - screenshots/fjsondb/shot-1.png
category: Developer Tools
summary: Tiny JSON file database for Node.js and TypeScript. Save and read data by key in one plain JSON file, with no database server to run
tags: [JSON database, Node.js database, Key value store, TypeScript, npm, Local storage, CLI, Developer tools]
website: https://github.com/p32929/fjsondb
source: https://github.com/p32929/fjsondb

platforms:
  Library: https://www.npmjs.com/package/fjsondb
---

fjsondb is a small JSON file database for Node.js and TypeScript. For a CLI, a bot, a prototype or some config, setting up a real database is too much, and writing your own read-and-save code for a JSON file gets messy fast. fjsondb keeps your data in one plain JSON file and gives you simple `set`, `get`, `has` and `delete` calls, with no server to run.

I made it because I was doing a lot of automation with Playwright and other tools, and needed somewhere to store data so I could check it later. The other solutions felt bulky for that, so I made my own.

1. **Plain JSON on disk:** open the file in any editor and read it.
2. **Save any value:** numbers, text, true or false, and nested objects.
3. **Counters built in:** `incrementNumber` and `decrementNumber` create the key at 0 if it is missing.
4. **Find keys by value:** `getKeysByMatchedValue` gives you every key that holds a value.
5. **As many files as you like:** one database per file.
6. **TypeScript types included.**

Great for CLIs, bots, small tools and quick prototypes.

## Install

```bash
npm install fjsondb
```

```ts
import { Fjsondb } from 'fjsondb'

const db = new Fjsondb('./data/test.json')
db.set('name', 'Fayaz')
db.get('name') // 'Fayaz'
```
