---
title: SIIN
icon: screenshots/siin/icon.png
screenshots:
  - screenshots/siin/shot-1.png
category: Developer Tools
summary: Batch app installer for Windows, like Ninite but with your own list. Give it a list of apps and it downloads and installs them all silently
tags: [Batch installer, Silent install, Ninite alternative, Windows, Install apps, New PC setup, Rust, CLI]
website: https://github.com/p32929/siin
source: https://github.com/p32929/siin

platforms:
  Windows: https://github.com/p32929/siin/releases/latest
  CLI: https://crates.io/crates/siin
---

SIIN is a batch app installer for Windows, a bit like Ninite, but you choose the apps. Setting up a new PC usually means downloading and clicking through one installer after another. With SIIN you write your list of apps once, and it downloads and installs them all silently, one after another, while you do something else.

1. **Your own list:** put any apps you want in a simple JSON file, with a direct download link for each.
2. **Installs everything silently,** one after another, with no clicking through installers.
3. **Custom install options:** pass extra arguments to an installer when you need to.
4. **Keep your list online:** host it on a GitHub Gist, npoint.io or Pastebin and use it on every new PC.

Great for setting up a new or freshly reset Windows PC, or the same apps on many computers.

Download the `.exe` from the download page and run it as administrator, or install it with `cargo install siin`. Then paste the link to your app list and press Enter.
