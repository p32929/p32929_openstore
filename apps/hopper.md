---
title: Hopper
icon: screenshots/hopper/icon.png
screenshots:
  - screenshots/hopper/1.png
  - screenshots/hopper/2.png
  - screenshots/hopper/3.png
  - screenshots/hopper/4.png
  - screenshots/hopper/5.png
  - screenshots/hopper/6.png
category: Developer Tools
summary: Zero-dependency self-hosted file manager. Manage any server's files from your browser or phone, with no npm packages that could be hijacked
tags: [Zero dependencies, Supply chain safe, File manager, Web file manager, Self-hosted, File upload, File sharing, Home server, Raspberry Pi, Open source]
website: https://github.com/p32929/hopper
source: https://github.com/p32929/hopper
license: MIT

platforms:
  Web: https://github.com/p32929/hopper
---

Hopper is a free, self-hosted web file manager with zero dependencies. Getting files on or off a computer or server usually means setting up FTP, installing a client or going through a cloud drive, and it's even harder from a phone. With Hopper you run one command on the machine, open its address in any browser, and manage its files right there.

What makes it different: other web file managers pull in dozens or hundreds of npm packages, and one hijacked package is all it takes to read every file on your server. Hopper uses only Node.js itself. There is nothing to `npm install`, no CDN scripts, and every line that touches your files is in one small repo you can read.

1. **Browse folders** in a list or a grid, sort them and filter by name.
2. **Upload files or whole folders** with a button or drag and drop. Big uploads carry on after a network hiccup.
3. **Download one file, or many at once** as a single ZIP.
4. **Open files in the browser:** images, video, audio, PDF and any text or code file.
5. **Create folders, rename and delete,** with a confirmation first.
6. **Works well on a phone or tablet,** with light and dark mode.

Handy for a home server, a Raspberry Pi, a remote machine, or just sending files from your phone to your computer.

I made Hopper because I kept moving files between Google Cloud and my own computer, and doing it over SSH was more complicated than it needed to be. So I made something simpler.

## Run it

```bash
git clone https://github.com/p32929/hopper.git
cd hopper
FM_PASSWORD='something long' node server.js
```

Then open `http://<your-machine>:3999`. It needs Node.js 18 or newer. Always set a password, or anyone on your network can change your files.

Want to buy the source code of this app? Contact me through my portfolio: https://p32929.github.io
