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
summary: A self-hosted web file manager with no dependencies. Browse, upload, download, preview and organise files on any machine from any browser, phone included
tags: [File manager, Self-hosted, Node.js, Upload, Download, Zero dependencies, Password, Open source]
website: https://github.com/p32929/hopper
source: https://github.com/p32929/hopper
license: MIT

platforms:
  Web: https://github.com/p32929/hopper
---

**Run one command on a machine, and manage its files from any browser.**

Hopper is a small file manager that lives on a computer or server. Start it with Node.js, open its address on your laptop or phone, and you can look through folders, move files in and out, and tidy things up. There is nothing to install: no packages, no database, just `node server.js`.

## Why I made it

I wanted a quick way to move files to and from a machine without setting up FTP, SFTP or a full cloud drive. It started as a tiny upload page and grew into a proper file manager that also works well on a phone.

## What you can do

1. Browse folders in a list or a grid, sort them, and filter by name. Hidden files are shown faded when you turn them on.
2. Upload files or whole folders by button or drag and drop. Big files go up in pieces and carry on after a network hiccup. You see the speed, the time left, and can cancel.
3. Download one file, or pick several files and folders and get them as a single ZIP.
4. Open files right in the browser instead of downloading them: images, video, audio, PDF, and any text or code file, with colours and line numbers. Use the arrow keys to go to the next file.
5. Create folders, rename and delete, with a confirmation first.
6. Use it on a phone or tablet. It has a menu drawer, a + button for adding files, and an action bar at the bottom when you select things.
7. Switch between light and dark mode.

## Keep it safe

You can set a password with `FM_PASSWORD='something long' node server.js`. Without it, anyone who can reach the port can change your files, so only run it on a network you trust.

With a password, visitors see a sign-in page and nothing else. After 5 wrong passwords, that visitor's address and browser are blocked for 7 days, or until you restart the server. You can also lock Hopper to one folder with `FM_ROOT`.

## Run it

```bash
git clone https://github.com/p32929/hopper.git
cd hopper
node server.js
```

Then open `http://<your-machine>:3999`. It needs Node.js 18 or newer.
