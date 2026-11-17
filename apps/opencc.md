---
title: opencc
icon: screenshots/opencc/icon.png
screenshots:
  - screenshots/opencc/shot-1.png
  - screenshots/opencc/shot-2.png
  - screenshots/opencc/shot-3.png
category: Developer Tools
summary: Use Claude Code with free or local models. A zero-dependency proxy that sends it to any OpenAI-compatible API and switches models when one fails
tags: [Claude Code, Claude Code proxy, OpenAI compatible, Free models, Local LLM, OpenRouter, Zero dependencies, Supply chain safe, AI coding]
website: https://github.com/p32929/opencc
source: https://github.com/p32929/opencc

platforms:
  CLI: https://github.com/p32929/opencc
---

opencc lets you use Claude Code with any OpenAI-compatible API, so you can code with free tiers, cheap providers or local models instead of paying for Anthropic. A small proxy runs on your computer and translates between the two. Claude Code doesn't notice.

What makes it different: other Claude Code proxies pull in many npm packages, and a proxy sees your code and your API keys. opencc uses only Node.js itself: no packages, nothing to `npm install`, so there is no supply chain for anyone to poison. It also does one job well. Add many free providers, and it learns which models actually work and sends each request to the best one.

1. **Claude Code on any model:** OpenRouter, Groq, Gemini, local servers, anything that speaks the OpenAI API.
2. **Never stuck on one model:** when a model fails, is rate limited or is too small for the request, the next best one answers.
3. **Learns as you work:** it keeps a record of what each model did, so the ones that work move up and the ones that fail move down.
4. **Smart about each request:** a request with tools, images or a PDF goes only to models that can handle it.
5. **Web panel** to add providers, pick and order your models, test them, and see every request it served.
6. **Works with HeartCode:** both use the same config file.

Great for anyone who likes Claude Code but wants to run it on free or local models.

I made opencc because I wanted to use Claude Code with free and local models.

## Run it

You need Node.js 18 or newer.

```bash
git clone https://github.com/p32929/opencc.git
cd opencc
npm start
```

Then run `opencc` and leave it running, and in your project folder run `opencc claude`. Add your providers in the panel it shows (`localhost:3450`).

Want to run AI coding tools on your own models? Contact me through my portfolio: https://p32929.github.io
