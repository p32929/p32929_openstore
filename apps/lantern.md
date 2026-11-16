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
summary: Checking a home server means SSH and remembered commands. One web page to see and control everything on your Linux box, with logs, buttons and a terminal
tags: [Self-hosted, Linux, Server, Monitoring, Dashboard, Terminal, Logs, Homelab, Open source]
website: https://github.com/p32929/lantern
source: https://github.com/p32929/lantern

platforms:
  Web: https://github.com/p32929/lantern
---

**Checking on your home server means SSH, remembered commands and hunting for logs. Lantern puts it all on one web page.**

## The problem

I have a small server at home (an old laptop, a Raspberry Pi, a mini PC) running a handful of things: a few containers, a couple of services, a script or two. To check on them I had to SSH in, try to remember the service name, read logs with one command, restart with another, and forget which port it used. None of that works well from a phone.

## How Lantern solves it

Lantern puts everything on one page you can open from your phone or laptop. Lantern is two files: a bash script and an HTML page. There is nothing to install, no database and no Docker. Run the script, open the address, and you can see and fix everything on that machine.

1. **See everything at a glance.** Each service is a row: green or red, its link, and how much CPU and memory it uses. The top shows the machine itself: CPU, memory, disk, uptime, Wi-Fi and battery.
2. **Fix things in one click.** Put a Restart, Deploy or any other button right on the row. Click it, a spinner turns, and you get "done" or the error.
3. **See how things have been doing.** Small graphs show the last hour of CPU and memory for every service, and the last day for the machine. Open a service for bigger 1, 6 and 24-hour charts.
4. **Read the logs live.** They update every second while you look.
5. **A real terminal in the browser.** `git pull` asks for a password? Type it. Ctrl-C, tab completion, colours and history all work. The shell keeps running when you close the page.
6. **Works with anything.** Lantern does not know about Docker or systemd. You give it a few shell commands per service, so it works for containers, services, plain processes, cron jobs or a game server. One-click templates cover the common ones.
7. **Buttons with icons.** Pick from more than 1,600 icons with a search ("deploy" finds rockets, "restart" finds arrows).
8. **Made for phones.** On a small screen every service becomes a card with the same information.
9. **Light and dark mode**, or follow your system.

## Get it running

You need Linux with bash and busybox, which are already on Ubuntu and Debian.

```bash
git clone https://github.com/p32929/lantern.git
cd lantern
./lantern.sh
```

It asks for a port, an optional PIN, and whether to keep running always (start on boot, come back after a crash). Then open the address it prints from any device on your network.

## Good to know

Lantern is made for your home network. Everything needs the PIN, including just looking. After 5 wrong PINs a device is locked out for 7 days. Commands and the terminal run as your user, and the connection is plain HTTP, so do not open it to the internet. To reach it from away from home, use a VPN such as Tailscale or WireGuard, or an SSH tunnel. It runs fine on very small machines, and I tested it on a Chromebook with 3 GB of RAM.
