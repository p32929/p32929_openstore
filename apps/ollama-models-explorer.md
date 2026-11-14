---
title: Ollama Models Explorer
icon: screenshots/ollama-models-explorer/icon.png
screenshots:
  - screenshots/ollama-models-explorer/1.png
  - screenshots/ollama-models-explorer/2.png
  - screenshots/ollama-models-explorer/3.png
  - screenshots/ollama-models-explorer/4.png
  - screenshots/ollama-models-explorer/5.png
  - screenshots/ollama-models-explorer/6.png
  - screenshots/ollama-models-explorer/7.png
  - screenshots/ollama-models-explorer/8.png
  - screenshots/ollama-models-explorer/9.png
  - screenshots/ollama-models-explorer/10.png
  - screenshots/ollama-models-explorer/11.png
category: Developer Tools
summary: Find the right Ollama model. Search 17,000+ models, see which run on your computer and how fast, compare them, and copy the install command
tags: [Ollama, AI models, LLM, Model browser, Compare, Search, Mobile friendly, Next.js, Dark mode]
website: https://ollama-models-explorer.vercel.app/
source: https://github.com/p32929/ollama_models_explorer

platforms:
  Web: https://ollama-models-explorer.vercel.app/
---

**Find the right Ollama model for your computer.**

Ollama's own website does not show what you need to choose a model when you do not have high-end hardware. This app was built to fix that. It lists every model, says which ones can run on your computer and how fast, and lets you narrow 17,000+ models down to the few worth trying.

## What it does

1. **Every model on Ollama.** The 270 official models, plus more than 17,000 community models uploaded by other people (named `user/model`). Switch between **All**, **Official** and **Community**.
2. **Will it run on my computer, and how fast?** The page works out your graphics card or Apple chip by itself, so you type nothing. Each model is marked **Can run well**, **Barely fits**, **Too big to run** or **Cloud**, with an estimate of **tokens per second** (about three quarters of a word each). If the guess is off, one tap picks the closest computer. One switch hides every model that cannot run, and you can sort or filter by speed.
3. **"I want to" picks**: Coding, Small and fast, Images, Reasoning, Embeddings, Translation, Chat and roleplay, Math, Tool use. Pick several at once and every model must match all of them.
4. **Every row shows the facts up front.** The size range (like 8B to 405B), the download size, and whether the model is **Dense** or **MoE** (mixture of experts, which is faster than its size suggests). No clicking needed.
5. **Click any model** for its details: will it run and how fast, the exact install command with a copy button (including the best version for your computer), every version with its size and speed, context window, downloads and more.
6. **Hover anything** for a plain-words explanation of what a badge, number or heading means and how it was worked out.
7. **Compare** up to four models side by side: sizes, context window, speed, downloads, last update, and whether each runs on your computer.
8. **What's new and Trending.** See models added or updated in the last two weeks, and what is rising.
9. **Search and filters.** Search by any words. Filter by capabilities (also several at once), how recently a model was updated, size, context window, or publisher, and hide near-duplicate community copies. Sort by downloads, update date, name, size or context.
10. **Search Ollama live** when you cannot find something. The saved list can be a few days old, and this asks ollama.com directly.
11. **Share a link.** Your search, filters and comparison are saved in the address.
12. **Made for phones.** Models become cards, filters open as a bottom sheet, comparing goes full screen, and every button is easy to tap.
13. **Light and dark mode**, a model of the week, a free JSON API and an RSS feed of new models.

## Good to know

The list is long, so rows load as you scroll. A script rebuilds the full list every week, so new models show up after the next refresh. The **Refresh Data** button re-reads the official models with all their versions. "Runs on my computer" and the speed are estimates, because browsers hide exact hardware. Speed is worked out from your memory speed and the model's size, so expect it to be within about a third of what you really get. Official models use their real download sizes, and the rest are estimated from the parameter count.

**Please self-host it if you can.** The public site runs on a free host, so it is not very fast and not always up. A copy on your own computer is faster and takes a minute: clone the repository, run `yarn install`, then `yarn dev`.
