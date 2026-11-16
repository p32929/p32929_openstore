---
title: CMDN
icon: screenshots/cmdn/icon.png
screenshots:
  - screenshots/cmdn/1.png
category: Developer Tools
summary: Get notified when a long terminal command finishes. Put cmdn in front of any command and hear a sound, or send a webhook, when it is done
tags: [Command line, CLI, Notification, Terminal, Long running command, Webhook, Developer tools, Windows, macOS, Linux]
website: https://github.com/p32929/cmdn
source: https://github.com/p32929/cmdn

platforms:
  CLI: https://github.com/p32929/cmdn
---

CMDN tells you when a long terminal command is done. Builds, installs and uploads can take minutes, and you either sit watching the terminal or forget about it and come back much later. Put `cmdn` in front of any command, and you get a sound the moment it finishes, so you can do something else in the meantime.

1. **Works with any command:** `cmdn npm install`, `cmdn docker build -t myapp .`, `cmdn git push` and so on.
2. **A sound when it finishes,** and you can use your own sound file.
3. **Run something after it ends:** send a webhook, write to a log file or show a desktop notification, with the command and its output included.
4. **Works on Windows, macOS and Linux.**
5. **Quick setup:** answer three questions, and change them any time with `cmdn --configure`.

Great for developers who run long builds, installs or deploys.

## Install

```bash
git clone https://github.com/p32929/cmdn.git
cd cmdn
npm install
npm run setup
```
