---
title: one console log
icon: screenshots/one-console-log/icon.png
screenshots:
  - screenshots/one-console-log/shot-1.png
category: Developer Tools
summary: VS Code extension that adds one clean console.log line for the variable under your cursor. A lighter take on Turbo Console Log
tags: [VS Code extension, console.log, JavaScript, TypeScript, Debugging, Turbo Console Log, Developer tools]
website: https://marketplace.visualstudio.com/items?itemName=p32929.one-console-log
source: https://github.com/p32929/one-console-log

platforms:
  Extension: https://marketplace.visualstudio.com/items?itemName=p32929.one-console-log
---

one console log is a VS Code extension that writes a `console.log` for you in one line. Typing logs by hand while debugging JavaScript or TypeScript is slow, and Turbo Console Log adds several lines each time, which clutters your code and your output. This one adds a single line with the file name and the variable, so your logs stay short and easy to clean up.

It's a fork of Turbo Console Log. The original adds several lines for each log; I wanted just one.

1. **One line per log:** a single `console.log` instead of several.
2. **Knows what to log:** put your cursor on a variable or a line and it logs that.
3. **Clear labels:** each log shows the file and the variable name, so you know where it came from.
4. **Same habit as Turbo Console Log,** with less noise.
5. **Free.**

Great for JavaScript and TypeScript developers who debug with `console.log` all day.

Install it from the VS Code Marketplace, or run `ext install p32929.one-console-log`. Then open the command palette and pick "Add console.log in this line". It only adds logs for now; for commenting or deleting all logs, use Turbo Console Log.

Want a VS Code extension that fits the way you code? Contact me through my portfolio: https://p32929.github.io
