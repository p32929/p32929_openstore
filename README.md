<h1 align="center">OpenStore</h1>
<p align="center"><b>Software made by people, not app stores.</b><br>
An open catalog of apps, tools and libraries. Every developer keeps their listing in their own GitHub repo.</p>
<p align="center"><a href="https://openstore.pfay.workers.dev"><b>Open the store →</b></a> &nbsp;·&nbsp; <a href="https://openstore.pfay.workers.dev/add"><b>Add your apps</b></a> &nbsp;·&nbsp; <a href="https://openstore.pfay.workers.dev/why">Why OpenStore</a></p>

<p align="center">
  <a href="https://openstore.pfay.workers.dev"><img src="docs/store-desktop.png" alt="OpenStore on desktop" width="68%"></a>
  <a href="https://openstore.pfay.workers.dev"><img src="docs/store-mobile.png" alt="OpenStore on mobile" width="22%"></a>
</p>

## Why you might want this

Good apps keep disappearing. Stores change their rules, remove old apps, and can close a developer account without a warning.

OpenStore is a different deal:

1. **Free.** No fees. No testers to find. No waiting for approval when you update an app.
2. **Yours.** Your listing is a few text files in your own public GitHub repo. Nobody can take it away.
3. **Everything in one place.** Web, Android, iOS, desktop, libraries, bots. Link to wherever your app already lives.

## How it works

1. **Copy the template.** Get the [`template` branch](https://github.com/p32929/p32929_openstore/tree/template) into a new public repo.
2. **Add one file per app.** A short `.md` file in `apps/`: name, icon, screenshots, links.
3. **Check it.** Run `node validate.mjs`. It tells you the exact line to fix.
4. **Join once.** Open one pull request on [openstore_maintainers](https://github.com/p32929/openstore_maintainers).

After that, every push to your repo shows up on OpenStore within a day.

An app file looks like this:

```yaml
---
title: My App
icon: images/icon.png
screenshots: [images/screenshot.png]
category: Productivity
platforms:
  Web: https://my-app.example.com
---

What it does, in plain Markdown.
```

## This repo

This is my own listing: the real one, with my apps, as a working example. Every `.md` file in [`apps/`](apps/) is an app, and its file name becomes its link. [`profile.yaml`](profile.yaml) is my developer page.

Want the same for yourself? Start from the [`template` branch](https://github.com/p32929/p32929_openstore/tree/template), not from this one.

Before pushing changes here:

```bash
node validate.mjs
```

## Links

1. [OpenStore](https://openstore.pfay.workers.dev) and [my listing](https://openstore.pfay.workers.dev/dev/p32929)
2. [Join the list](https://github.com/p32929/openstore_maintainers)
3. [Bugs, ideas and questions](https://github.com/p32929/openstore_feedback)

## Contributing

Ideas and fixes are very welcome, thank you! Before you start on a pull request, please open an issue in [openstore_feedback](https://github.com/p32929/openstore_feedback) and tell me what you would like to add or change. That way we can agree on it first, and your time is not wasted on something that might not fit.

## You might also like

<p><a href="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/0"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/0-dark.svg"><img src="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/0-light.svg" width="50%" align="top" alt="More apps by p32929 on OpenStore (1)"></picture></a><a href="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/1"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/1-dark.svg"><img src="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/1-light.svg" width="50%" align="top" alt="More apps by p32929 on OpenStore (2)"></picture></a><br><a href="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/2"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/2-dark.svg"><img src="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/2-light.svg" width="50%" align="top" alt="More apps by p32929 on OpenStore (3)"></picture></a><a href="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/3"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/3-dark.svg"><img src="https://openstore.pfay.workers.dev/more/p32929/p32929_openstore/3-light.svg" width="50%" align="top" alt="More apps by p32929 on OpenStore (4)"></picture></a></p>

<p><a href="https://p32929.github.io/share/?repo=p32929_openstore"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-share-dark.svg"><img src="https://p32929.github.io/readme/footer-share-light.svg" width="50%" align="top" alt="Share this project with your friends in one click"></picture></a><a href="https://p32929.github.io/support/"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-support-dark.svg"><img src="https://p32929.github.io/readme/footer-support-light.svg" width="50%" align="top" alt="If you like my work and want to support me, feel free to support"></picture></a><br><a href="https://openstore.pfay.workers.dev/add"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-join-dark.svg"><img src="https://p32929.github.io/readme/footer-join-light.svg" width="100%" align="top" alt="Put your own apps on OpenStore: free, your listing lives in your own repo"></picture></a></p>

