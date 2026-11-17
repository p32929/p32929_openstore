---
title: oaifai
icon: screenshots/oaifai/icon.png
screenshots:
  - screenshots/oaifai/shot-1.png
  - screenshots/oaifai/shot-2.png
category: Utilities
summary: Connect Ubuntu Server to WiFi from a simple terminal list, without NetworkManager or hand-written netplan files. Rolls back if it fails
tags: [WiFi, Ubuntu Server, Netplan, Linux, Terminal UI, TUI, CLI, Headless server, Raspberry Pi, Rust]
website: https://github.com/p32929/oaifai
source: https://github.com/p32929/oaifai
license: MIT

platforms:
  CLI: https://github.com/p32929/oaifai/releases/latest
---

oaifai is a small terminal app to scan for WiFi and connect on Ubuntu Server and other netplan systems that have no NetworkManager. Normally that means editing netplan YAML files by hand and hoping the indentation is right. With oaifai you pick a network from a list, type the password, and it writes the config for you. The name is how "WiFi" sounds in Bangla.

What makes it different: changing WiFi on a headless server is risky, because one wrong setting can cut you off. oaifai saves a backup of your netplan file before it changes anything, and if the new network does not connect within about 20 seconds, it puts your old settings back by itself. It is one small program with a single library behind it, so there is very little to install or trust.

1. **Networks in a list,** with signal strength and the one you are connected to.
2. **Type the password and connect.** Leave it empty for open networks, or enter a hidden network's name by hand.
3. **Safe changes:** backup first, then automatic rollback if it can't connect.
4. **Disconnect with one key,** `d`, anywhere.
5. **Scriptable too:** `--list`, `--connect` and `--disconnect` without the screen, plus `--dry-run` to see the config without applying it.

Great for home servers, mini PCs and Raspberry Pi style machines running Ubuntu Server.

I made oaifai after I installed a Linux server on a Chromebook, where connecting to WiFi was a pain. I know there are plenty of tools for this, but I wanted my own, so I wrote it in Rust.

Good to know: it is for Linux x86_64 with netplan, and right now it expects the WiFi interface `wlp1s0` and the netplan file `00-installer-config.yaml`. Pressing `d` drops your network straight away, which also ends an SSH session that uses it.

## Install

```sh
curl -fsSL https://raw.githubusercontent.com/p32929/oaifai/master/install.sh | sh
```

Then run `oaifai`. It asks for your sudo password, because scanning and changing network settings need it. On other systems, build it from source with `cargo build --release`.

Want to buy the source code of this app? Contact me through my portfolio: https://p32929.github.io
