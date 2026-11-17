---
title: cccsss
icon: screenshots/cccsss/icon.png
screenshots:
  - screenshots/cccsss/shot-1.png
  - screenshots/cccsss/shot-2.png
  - screenshots/cccsss/shot-3.png
category: Developer Tools
summary: Browse your Claude Code sessions in the terminal, read any of them, and resume one with the exact command. Zero dependencies
tags: [Claude Code, Session browser, Resume sessions, Terminal UI, TUI, CLI, Zero dependencies, Supply chain safe, npm]
website: https://github.com/p32929/cccsss
source: https://github.com/p32929/cccsss
license: MIT

platforms:
  CLI: https://www.npmjs.com/package/cccsss
---

cccsss is a terminal app to browse your Claude Code sessions and get the exact command to resume any of them. Claude Code keeps every conversation, but finding the right one later means guessing from IDs, and `claude --resume` only finds a session when you run it from the folder it started in. cccsss lists your sessions by their first prompt, lets you read them, and hands you the full `cd ... && claude --resume ...` command.

What makes it different: it reads files full of your code and conversations, so it is pure Node.js with zero dependencies. There are no third-party packages to install, so there is no supply chain for anyone to attack. The whole screen, lists, filtering, scrolling and search, is built on Node.js itself.

1. **Every project and session in one place,** with the first prompt as the title, message count, age and size.
2. **Read a whole conversation** before you resume it, and jump between your prompts or search inside it.
3. **Resume the right way:** copy the command with the `cd` included, or let cccsss run it for you.
4. **Pick a permission mode** for the resumed session, like plan or accept edits. It remembers your choice.
5. **Filter and sort** projects and sessions.
6. **Clean up safely:** delete old sessions or a whole project, only after you confirm. It never touches anything outside your Claude Code session files.

Great for anyone who uses Claude Code every day across many projects.

I made cccsss because I kept needing to find my old Claude Code sessions again. I wanted it to have zero dependencies and be easy to run, and to open the conversation for me instead of making me copy a session ID.

## Install

You need Node.js 18 or newer.

```bash
npm install -g cccsss
```

Then run `cccsss` in a project folder, or try it once with `npx cccsss`.

Want a custom version of this app, or help changing it for your needs? Contact me through my portfolio: https://p32929.github.io
