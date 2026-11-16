---
title: Lantern
icon: screenshots/lantern/icon.png
screenshots:
  - screenshots/lantern/1.png
  - screenshots/lantern/2.png
  - screenshots/lantern/3.png
  - screenshots/lantern/4.png
  - screenshots/lantern/5.png
  - screenshots/lantern/6.png
  - screenshots/lantern/7.png
category: Developer Tools
summary: Self-hosted Linux server dashboard. See status, CPU, memory and logs, restart services in one click, and use a terminal, all from one web page
tags: [Server dashboard, Linux, Homelab, Self-hosted, Server monitoring, Raspberry Pi, Logs, Web terminal, Open source]
website: https://github.com/p32929/lantern
source: https://github.com/p32929/lantern

platforms:
  Web: https://github.com/p32929/lantern
---

**Lantern is a free, self-hosted dashboard for your Linux server or homelab. See every service, its CPU, memory and logs, restart things in one click, and open a terminal, all from one web page on your phone or laptop.**

## The problem

Many people run a small server at home on an old laptop, a Raspberry Pi or a mini PC, with a few containers, services and scripts. To check on them you have to SSH in, remember the service name, read logs with one command, restart with another, and forget which port it used. None of that works well from a phone.

## How Lantern solves it

Lantern puts everything on one page. Run one script, open the address, and you can see and fix everything on that machine. There is no database and no Docker to set up.

1. **See everything at a glance:** each service is green or red, with its CPU and memory. The machine's CPU, memory, disk and uptime are at the top.
2. **Fix things in one click:** put a Restart, Deploy or any other button right on a service.
3. **See how things have been doing** with CPU and memory graphs for the last hour or day.
4. **Read the logs live.**
5. **Use a real terminal in the browser.**
6. **Works with anything:** Docker containers, system services, plain processes, cron jobs or a game server.
7. **Made for phones,** with light and dark mode.

## Who it is for

1. Homelab and self-hosting fans.
2. Raspberry Pi and home server owners.
3. Developers who run a few apps on one Linux machine.

## Get it running

```bash
git clone https://github.com/p32929/lantern.git
cd lantern
./lantern.sh
```

It asks for a port and a PIN, then prints the address to open. It runs on Ubuntu, Debian and most Linux machines, even very small ones. Use it on your home network only, not open to the internet; from outside, connect through a VPN such as Tailscale.
