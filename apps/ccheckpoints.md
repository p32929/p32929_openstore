---
title: CCheckpoints
icon: screenshots/ccheckpoints/icon.png
screenshots:
  - screenshots/ccheckpoints/shot-1.png
  - screenshots/ccheckpoints/shot-2.png
  - screenshots/ccheckpoints/shot-3.png
category: Developer Tools
summary: Checkpoints for Claude Code, like in Cursor. Saves every message of your coding sessions and shows them in a web dashboard to look back and compare
tags: [Claude Code, Checkpoints, AI coding, Cursor checkpoints, Session history, Developer tools, CLI, npm]
website: https://github.com/p32929/ccheckpoints
source: https://github.com/p32929/ccheckpoints

platforms:
  CLI: https://www.npmjs.com/package/ccheckpoints
---

CCheckpoints adds Cursor-style checkpoints to Claude Code CLI. In a long Claude Code session it is easy to lose track of what you asked and when things changed. CCheckpoints saves a checkpoint every time you send a message, and shows your whole session as a timeline in a web dashboard, so you can look back at any point.

I made it because Claude Code didn't have checkpoints back then. I looked for a solution, couldn't find one, and built it. Claude Code has its own checkpoints now, so you don't really need this anymore.

1. **Automatic checkpoints:** every message you send to Claude Code is saved, with the time.
2. **See all your sessions:** when you started, how long you worked, and what happened in each one.
3. **Checkpoint timeline:** move through your whole conversation with its full context.
4. **Compare changes** between checkpoints, to find what broke or see how your code changed.
5. **One command setup:** it sets up the Claude Code hooks for you and opens the dashboard.
6. **Stays on your computer:** everything is saved locally.

Great for anyone who codes with Claude Code and misses Cursor's checkpoints.

## Install

```bash
npm install -g ccheckpoints
ccheckpoints
```

You can also use the short name `ccp`.

Want a tool that fits the way you work with AI coding agents? Contact me through my portfolio: https://p32929.github.io
