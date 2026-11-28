---
title: tabrider
icon: screenshots/tabrider-example/icon.png
screenshots:
  - screenshots/tabrider-example/shot-1.png
  - screenshots/tabrider-example/shot-2.png
category: Developer Tools
kind: personal
featured: true
summary: Browser automation library for Chrome extensions with a Playwright-style API. Run automation scripts in your real browser so sites don't flag them as bots
tags: [Browser automation, Chrome extension, Playwright alternative, Puppeteer alternative, Web scraping, Form filling, Bot detection, TypeScript, npm, Developer tools]
website: https://www.npmjs.com/package/tabrider

platforms:
  Library: https://www.npmjs.com/package/tabrider
---

tabrider is a browser automation library for Chrome extensions with a Playwright-style API, so your automation scripts run inside your own extension, in your real browser, instead of in an automated browser that websites can detect and block.

What makes it different: tools like Playwright and Puppeteer start a separate, automated browser, and many websites can tell and flag it as a bot. tabrider runs inside a normal Manifest V3 extension in the browser you already use, so sites see a regular browser. There is no separate driver, no server and no second browser to manage, and you can ship your automation to others as an extension.

1. **Playwright-style commands:** open, close and switch tabs, go to a URL, click, double-click, right-click, hover, type, fill, select, check, drag and drop, press keys and wait for elements.
2. **CSS selectors and XPath** both work.
3. **Fill a whole form in one call** with `fillForm`.
4. **Scrape data:** get text from one element or many, or collect several fields into an object with `scrapeData`.
5. **Downloads and uploads:** wait for a download, or upload a file to a form.
6. **Run your own JavaScript in the page** with `evaluate`.
7. **Human-like delays** with `randomWait`.
8. **Jobs and progress:** run named jobs and track their progress, with state saved to Chrome storage.
9. **Built-in logging.**
10. **Clear error handling:** every command returns a result you can check, instead of throwing.

I made tabrider because I was doing browser automation with Playwright, and many websites could detect it was an automated browser. I tried many things, but they kept detecting it. So I thought: what if it ran as a Chrome extension? Websites usually treat extensions as normal, not as bots, and so far it works.

Great for developers who want to automate repetitive work in Chrome, like filling forms or collecting data, and make their automation scripts easier to write.

## Install

```bash
npm install tabrider
```

Your extension's `manifest.json` needs the permissions `activeTab`, `storage`, `tabs` and `scripting`, and the host permission `*://*/*`.

The easiest way to start is the example extension, a complete Chrome extension that uses tabrider: https://github.com/p32929/tabrider_example

Want a browser automation built for your workflow? Contact me through my portfolio: https://p32929.github.io
