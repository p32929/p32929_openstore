---
title: Fay
icon: screenshots/fay/icon.png
screenshots:
  - screenshots/fay/shot-1.png
category: Developer Tools
summary: Save a list of shell commands under one name and run them all again from a menu. A small command line tool for Windows, macOS and Linux
tags: [Command line, CLI, Shell commands, Automation, Bash, CMD, Rust, Developer tools]
website: https://github.com/p32929/fay_cli
source: https://github.com/p32929/fay_cli

platforms:
  CLI: https://crates.io/crates/fay
---

Fay is a small command line tool that saves a series of shell commands under one name, so you can run them all again with one pick. If you keep typing the same setup, build or deploy steps one by one, Fay remembers them for you. Just type `fay`, choose the saved list from a menu, and it runs every command in order.

1. **Save a list of commands** under a name, and run the whole list with one pick.
2. **Easy menu:** no flags to remember, just run `fay` and follow the steps.
3. **Works everywhere:** the same tool runs with bash or cmd on Windows, macOS and Linux.
4. **Easy to back up:** your saved commands are kept in a plain JSON file.

Great for developers who run the same few commands every day.

## Install

```bash
cargo install fay
```

Then type `fay` and press Enter.
