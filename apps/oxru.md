---
title: Oxru
icon: screenshots/oxru/icon.png
screenshots:
  - screenshots/oxru/shot-1.png
  - screenshots/oxru/shot-2.png
  - screenshots/oxru/shot-3.png
category: Developer Tools
summary: Lightweight code editor for the terminal or its own window, with all of a project's terminals inside it. Uses a fraction of VS Code's memory
tags: [Code editor, Terminal editor, Lightweight editor, Rust, VS Code alternative, Terminal multiplexer, SSH, Open source]
website: https://github.com/p32929/oxru
source: https://github.com/p32929/oxru
license: MIT

platforms:
  CLI: https://github.com/p32929/oxru
---

Oxru is a small, fast code editor that runs in your terminal or in its own window, with all of a project's terminals living inside it. A project with a backend, a bundler and an app usually leaves a pile of terminal windows scattered across your desktop, while VS Code eats your memory. Oxru keeps the files and every terminal in one light window.

I made it because a project with a backend, a bundler and an app left terminal windows everywhere, and VS Code ate my memory. I wanted the files and every terminal together in one light window.

What makes it different: it is one native binary with no Electron, so it stays light (about 12 MB of memory on its start screen when we ran it). The same editor works as a desktop window and inside a plain terminal over SSH, with the same keys, and there is nothing to configure.

1. **Every terminal in one place:** open as many as you need as tabs, or see them all at once in a grid. A script that opens several terminals opens them inside Oxru instead.
2. **Window or terminal, same app:** it opens a window by default and runs in your terminal with `--term`, which also works over SSH.
3. **Fast file picker:** type to search your project, or browse the tree, create, rename and delete files.
4. **Syntax highlighting** for Rust, JavaScript, TypeScript, Python, Go, C, HTML, CSS, JSON, Bash and TOML.
5. **Multiple cursors, word wrap and tabs** for your open files.
6. **Light on purpose:** the status bar shows live memory use, and you can slow down terminal redraws to save CPU.
7. **Pick a font size and theme color** in Settings.

Great for developers who live in the terminal and want something lighter than VS Code without setting up Neovim.

## Install

You need a Rust toolchain (`cargo`). This builds Oxru from source and puts `oxru` on your PATH:

```bash
curl -fsSL https://raw.githubusercontent.com/p32929/oxru/master/install.sh | sh
```

Then run `oxru` in your project folder, or `oxru --term` to stay in the terminal.

Want a custom version of this app, or help changing it for your needs? Contact me through my portfolio: https://p32929.github.io
