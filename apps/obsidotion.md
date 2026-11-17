---
title: obsidotion
icon: screenshots/obsidotion/icon.svg
screenshots:
  - screenshots/obsidotion/shot-1.png
  - screenshots/obsidotion/shot-2.png
category: Productivity
summary: Obsidian Notion sync plugin. Send your vault to a Notion database and pull Notion edits back, on desktop and mobile. Only touches pages it made
tags: [Obsidian plugin, Notion, Obsidian to Notion, Notion sync, Notes sync, Markdown, Android, Open source]
website: https://github.com/p32929/obsidotion
source: https://github.com/p32929/obsidotion

platforms:
  Extension: https://github.com/p32929/obsidotion/releases/latest
---

obsidotion is an Obsidian plugin that syncs your notes with a Notion database. If you write in Obsidian but share or read your notes in Notion, copying them over by hand gets old fast. With two buttons you send your notes to Notion and bring changes made in Notion back.

I made it because Obsidian's official sync is paid, and I wanted a free option. So I made one that syncs through Notion.

1. **Upload to Notion:** sends new and changed notes to your Notion database. Unchanged notes are skipped, so it is quick.
2. **Pull from Notion:** brings edits made in Notion back into your notes, and adds new Notion pages as notes. It asks once before changing anything.
3. **Safe with your Notion:** it only updates or removes pages it made itself. Pages you created in Notion are never touched.
4. **Keeps your note properties,** like tags and other frontmatter, as they are.
5. **Long notes work too,** with headings, lists, checkboxes, quotes, code and tables.
6. **Works everywhere Obsidian runs,** on Windows, Mac, Linux, Android and iPhone.
7. **Free and open source.**

Great for people who keep notes in Obsidian but also need them in Notion.

Version 1.1.0 (2026) fixed a bug where uploading could remove pages you made in Notion, and added the pulling of new Notion pages. To set it up, you create a Notion integration and connect it to a database. The project page has the steps.

Download `obsidotion-plugin.zip` from the download page. In your vault, make the folder `.obsidian/plugins/obsidotion`, put the 3 files from the zip in it, then turn the plugin on in Obsidian's Community plugins.

Want a custom version of this app, or help changing it for your needs? Contact me through my portfolio: https://p32929.github.io
