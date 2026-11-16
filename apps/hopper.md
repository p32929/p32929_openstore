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

**Hopper is a free, self-hosted web file manager. Run one command on any computer or server, then browse, upload, download and preview its files from any browser, even on your phone.**

## The problem

Moving files to and from a computer or server is often a chore. You have to set up FTP or SFTP, install a client, or upload everything to a cloud drive first. From a phone it is even harder.

## How Hopper solves it

Start Hopper on the machine and open its address on your laptop or phone. You can look through folders, move files in and out, and tidy things up, all in the browser. There is nothing else to install.

1. **Browse folders** in a list or a grid, sort them, and filter by name.
2. **Upload files or whole folders** with a button or drag and drop. Big uploads carry on after a network hiccup, and you see the speed and time left.
3. **Download one file, or many at once** as a single ZIP.
4. **Open files right in the browser:** images, video, audio, PDF, and any text or code file.
5. **Create folders, rename and delete,** with a confirmation first.
6. **Works well on a phone or tablet.**
7. **Light and dark mode.**

## Who it is for

1. People with a home server, Raspberry Pi or old laptop who want to move files to it.
2. Developers who need to get files on or off a remote machine quickly.
3. Anyone who wants to send files from a phone to a computer without a cloud drive.

## Run it

```bash
git clone https://github.com/p32929/hopper.git
cd hopper
FM_PASSWORD='something long' node server.js
```

Then open `http://<your-machine>:3999`. It needs Node.js 18 or newer. Always set a password: without one, anyone on your network can change your files.
