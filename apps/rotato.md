---
title: rotato
icon: screenshots/rotato/icon.png
screenshots:
  - screenshots/rotato/1.png
  - screenshots/rotato/2.png
  - screenshots/rotato/3.png
category: Developer Tools
summary: Zero-dependency API key rotator for OpenAI, Gemini, Groq and OpenRouter. Switches keys on rate limits, with no npm packages to steal your keys
tags: [API key rotation, Zero dependencies, Supply chain safe, LLM proxy, OpenAI, Gemini, Groq, OpenRouter, Rate limit, Self-hosted]
website: https://github.com/p32929/rotato
source: https://github.com/p32929/rotato
license: MIT

platforms:
  Web: https://github.com/p32929/rotato
---

rotato is a small self-hosted proxy that rotates your API keys for OpenAI, Gemini, Groq, OpenRouter and any OpenAI or Gemini compatible API. Free and cheap API keys hit their rate limit fast, and then your app stops with a 429 error. Put rotato in between, give it several keys, and when one key is limited it quietly tries the next one, so your app keeps working.

What makes it different: tools like this usually pull in hundreds of npm packages, and any one of them could be hijacked to steal the API keys you hand it. rotato uses only Node.js itself. There is nothing to `npm install`, no `node_modules`, and even the admin page's styles come from the repo, not a CDN. Every line that touches your keys is in one repo you can read.

1. **Switches keys on rate limits,** or on any error codes you choose, and avoids keys that just failed.
2. **Many providers at once:** each gets its own path, like `/groq` or `/gemini`. Point your app there instead of the provider.
3. **Streaming works,** so chat replies still arrive word by word.
4. **Admin page** to add, test, reorder and turn off keys and providers, without restarting.
5. **Request log** that shows which key worked and which failed.
6. **Optional access key** so only your apps can use your proxy.
7. **Optional outbound proxies,** including free public ones it finds and checks itself.
8. **Telegram bot** to chat with any of your models from your phone.

Great for side projects and hobby apps that run on free or low-tier API keys.

## Run it

```bash
git clone https://github.com/p32929/rotato.git
cd rotato
cp .env.example .env   # set PORT and ADMIN_PASSWORD
npm start
```

Then open `http://localhost:8990/admin`, add your keys, and point your app at the endpoint it shows.
