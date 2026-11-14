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
category: Developer Tools
summary: Find the right Ollama model. Search 17,000+ models, see which run on your computer and how fast, compare them, and copy the install command
tags: [Ollama, AI models, LLM, Model browser, Compare, Search, Mobile friendly, Next.js, Dark mode]
website: https://ollama-models-explorer.vercel.app/
source: https://github.com/p32929/ollama_models_explorer

platforms:
  Web: https://ollama-models-explorer.vercel.app/
---

**Find the right Ollama model without clicking through hundreds of pages.**

Ollama hosts a huge number of models, and its own site is slow to scan. Ollama Models Explorer puts every one of them in one fast table, and tells you which ones will actually run on your computer.

## What it does

1. **Every model on Ollama.** The 270 official models, plus more than 17,000 community models uploaded by other people (named `user/model`). Switch between **All**, **Official** and **Community**.
2. **Will it run on my computer, and how fast?** The page works out your graphics card or Apple chip by itself, so you type nothing. Each model is marked **Runs well**, **Tight fit**, **Too big** or **Cloud**, with an estimate of **tokens per second** (about three quarters of a word each). If the guess is off, one tap picks the closest computer. One switch hides everything that will not run, and you can sort or filter by speed.
3. **"I want to" picks**: Coding, Small and fast, Images, Reasoning, Embeddings, Translation, Chat and roleplay, Math, Tool use. Pick several at once and every model must match all of them.
4. **Click any model** for its details: will it run and how fast, the exact install command with a copy button (including the best version for your computer), every version with its size and speed, context window, downloads and more.
5. **Hover anything** for a plain-words explanation of what a badge, number or heading means and how it was worked out.
6. **Compare** up to four models side by side: sizes, context window, speed, downloads, last update, and whether each runs on your computer.
7. **What's new and Trending.** See models added or updated in the last two weeks, and what is rising.
8. **Search and filters.** Search by any words. Filter by capabilities (also several at once), how recently a model was updated, size, context window, or publisher, and hide near-duplicate community copies. Sort by downloads, update date, name, size or context.
9. **Search Ollama live** when you cannot find something. The saved list can be a few days old, and this asks ollama.com directly.
10. **Share a link.** Your search, filters and comparison are saved in the address.
11. **Made for phones.** Models become cards, filters open as a bottom sheet, comparing goes full screen, and every button is easy to tap.
12. **Light and dark mode**, a model of the week, a free JSON API and an RSS feed of new models.

## Good to know

The list is long, so rows load as you scroll. A script rebuilds the full list every week, so new models show up after the next refresh. The **Refresh Data** button re-reads the official models with all their versions. "Runs on my computer" and the speed are estimates, because browsers hide exact hardware. Speed is worked out from your memory speed and the model's size, so expect it to be within about a third of what you really get. Official models use their real download sizes, and the rest are estimated from the parameter count.

It is a Next.js app. To run it yourself, clone the repository, run `yarn install`, then `yarn dev`.
