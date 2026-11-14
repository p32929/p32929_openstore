---
title: s3cr3tm3
icon: screenshots/s3cr3tm3/icon.png
screenshots:
  - screenshots/s3cr3tm3/1.png
  - screenshots/s3cr3tm3/2.png
  - screenshots/s3cr3tm3/3.png
  - screenshots/s3cr3tm3/tablet-1.png
  - screenshots/s3cr3tm3/tablet-2.png
  - screenshots/s3cr3tm3/phone-1.png
  - screenshots/s3cr3tm3/phone-2.png
category: Communication
summary: Write a private note, send someone the link, and they read it once and delete it. No account, free, made for my own freelance work
tags: [Secret Messages, Private Notes, Share Link, Freelance, No Sign-up]
website: https://s3cr3tm3.netlify.app/

platforms:
  Web: https://s3cr3tm3.netlify.app/
---

I built this for myself when I worked as a freelancer. On sites like Fiverr and Upwork, you and your client are meant to talk inside the app, and I wanted an easy way for me and my client to share information back and forth, especially contact information. One of us writes a message, sends the link, and the other opens it, reads it and deletes it.

**So I made the simplest thing that works.** You type a message (up to 1000 characters) and press **Save**. You get a link. Send it to the other person. They open it, read the message, and press **Delete** when they're done. Either of you can delete it, from any device.

There's nothing to sign up for, nothing to install, and it's free. The page is one box and two buttons, so it takes a few seconds to use.

**What it's for.** My goal was simple: other people shouldn't be able to see what my client and I shared. Each message gets a long, random link that nobody can guess, and most people aren't hackers, so for me that was good enough.

**It was made just for me, so please know what it is and what it isn't.** I only built this for my own use and my own clients. I never planned for other people to use it, so I didn't put in the things a proper secret-message service would have. Two things to know:

1. **Delete hides the message; it doesn't erase it.** When someone presses Delete, the link stops working, but the text stays in the database. I never added real removal because I didn't need it.
2. **Messages are not encrypted.** They are stored as plain text, and anyone who has the link can read the message until it's deleted.

It's not built to stop someone who really knows how to look. So don't put anything truly sensitive in it, like bank details or passwords you can't change. It's fine for everyday things you'd be okay with going no further than the person you sent it to.

It's free to use, and if it's useful to you, you're welcome to it.
