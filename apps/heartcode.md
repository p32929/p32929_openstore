---
title: HeartCode
icon: screenshots/heartcode/icon.png
screenshots:
  - screenshots/heartcode/shot-1.png
  - screenshots/heartcode/shot-2.png
category: Developer Tools
summary: Zero-dependency coding agent for your terminal. Works with any OpenAI-compatible model, free or local, and switches models when one fails
tags: [Coding agent, AI coding CLI, Claude Code alternative, OpenAI compatible, Free models, Local LLM, Ollama, OpenRouter, Zero dependencies, Supply chain safe]
website: https://github.com/p32929/HeartCode
source: https://github.com/p32929/HeartCode
license: MIT

platforms:
  CLI: https://www.npmjs.com/package/heartcode
---

HeartCode is a coding agent for your terminal that works with any OpenAI-compatible model: free ones, paid ones, local ones, several at once. Most coding agents stop the moment their one model hits a rate limit or gets stuck. HeartCode moves the work to your next model and keeps going.

What makes it different: a coding agent runs with your files, your keys and your shell, yet most of them pull in hundreds of npm packages that could be hijacked in an update. HeartCode has zero dependencies, only Node.js and its own code, so there is nothing for anyone to poison. And it is built for free and small models: it guides models that can't call tools one simple step at a time.

1. **Keeps working when a model doesn't:** on a rate limit, an error, a too-long conversation or a model going round in circles, another of your models takes over.
2. **Picks the best model for the job:** it remembers how each model does in real work and uses public coding rankings to choose who takes over.
3. **Checks its own work:** it runs and tests what it changed, and another model reviews the result before it says "done".
4. **Good with small and local models,** including ones that can't call tools.
5. **Learns per project:** it saves notes and lessons so the next task starts smarter.
6. **Set up in a web page,** not config files. Skills, MCP servers and hooks in Claude Code's formats.
7. **Tabs, background servers and notifications** when a task finishes or needs you.

Great for developers who want a capable coding agent on free or local models, without trusting a pile of packages.

## Install

You need Node.js 22 or newer.

```bash
npm install -g heartcode
```

Then run `heart` in your project folder and type `/settings` to add your providers.
