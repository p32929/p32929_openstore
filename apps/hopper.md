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
summary: Self-hosted web file manager. Browse, upload, download and preview files on any computer or server from your browser or phone, with one command
tags: [File manager, Web file manager, Self-hosted, File upload, File sharing, Home server, Raspberry Pi, Open source]
website: https://github.com/p32929/hopper
source: https://github.com/p32929/hopper
license: MIT

platforms:
  Web: https://github.com/p32929/hopper
---

Hopper is a free, self-hosted web file manager. Getting files on or off a computer or server usually means setting up FTP, installing a client or going through a cloud drive, and it's even harder from a phone. With Hopper you run one command on the machine, open its address in any browser, and manage its files right there.

1. **Browse folders** in a list or a grid, sort them and filter by name.
2. **Upload files or whole folders** with a button or drag and drop. Big uploads carry on after a network hiccup.
3. **Download one file, or many at once** as a single ZIP.
4. **Open files in the browser:** images, video, audio, PDF and any text or code file.
5. **Create folders, rename and delete,** with a confirmation first.
6. **Works well on a phone or tablet,** with light and dark mode.

Handy for a home server, a Raspberry Pi, a remote machine, or just sending files from your phone to your computer.

## Run it

```bash
git clone https://github.com/p32929/hopper.git
cd hopper
FM_PASSWORD='something long' node server.js
```

Then open `http://<your-machine>:3999`. It needs Node.js 18 or newer. Always set a password, or anyone on your network can change your files.
