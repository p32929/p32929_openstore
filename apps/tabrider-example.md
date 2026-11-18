---
title: tabrider example
icon: screenshots/tabrider-example/icon.png
screenshots:
  - screenshots/tabrider-example/shot-1.png
  - screenshots/tabrider-example/shot-2.png
category: Developer Tools
kind: personal
summary: Example Chrome extension for tabrider, a Playwright-style browser automation library that runs inside your extension, in your real browser
tags: [Browser automation, Chrome extension, Playwright alternative, Web scraping, Form filling, TypeScript, npm, Open source]
website: https://github.com/p32929/tabrider_example
source: https://github.com/p32929/tabrider_example

platforms:
  Extension: https://github.com/p32929/tabrider_example
---

tabrider example is a complete Chrome extension that shows how to use tabrider, a browser automation library with a Playwright-style API that runs inside a Chrome extension. Tools like Playwright and Puppeteer start a separate browser and need Node.js running in the background. With tabrider, your automation lives in the extension itself and works in the browser you already use.

I made tabrider because I was writing browser automation with Playwright, and a lot of websites could tell it was an automated browser. I tried many things, but they kept detecting it. So I thought: what if it ran as a Chrome extension? Websites usually treat extensions as normal, not as bots, and so far it works.

What makes it different: you write automations with the familiar commands from Playwright (`click`, `fill`, `waitFor`, `goto`), but they run as part of a normal Manifest V3 extension. There is no separate server, no driver to install, and no second browser to manage, and you can ship your automation to others as an extension.

1. **Playwright-style commands:** open and close tabs, click, double-click, right-click, hover, type, fill, select, check, drag and drop, press keys and wait for elements.
2. **CSS selectors and XPath** both work.
3. **Fill a whole form in one call,** and scrape text from a page into an object with `scrapeData`.
4. **Downloads and uploads:** click and wait for a download, or upload a file to a form.
5. **Jobs and progress,** with state saved to Chrome storage.
6. **Clear error handling:** every command returns a result you can check, instead of throwing.
7. **A ready-made popup** to pick and run your automations, plus a small local server for the file demo.

Great for developers who want to automate repetitive work in the browser, like filling forms or collecting data, and share it as an extension.

To try it, you need Node.js. Clone the repository and run `./run_prod.sh`, then open `chrome://extensions`, turn on Developer mode, click **Load unpacked** and pick the `dist` folder. To use tabrider in your own extension, run `npm install tabrider`.

Want the boring work in your browser done for you? Contact me through my portfolio: https://p32929.github.io
