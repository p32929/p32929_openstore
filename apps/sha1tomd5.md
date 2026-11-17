---
title: Sha1ToMd5
icon: screenshots/sha1tomd5/icon.png
screenshots:
  - screenshots/sha1tomd5/shot-1.png
  - screenshots/sha1tomd5/shot-2.png
  - screenshots/sha1tomd5/shot-3.png
category: Developer Tools
summary: Get the Facebook Login key hash for your Android app from its SHA-1 in one paste. No logging code, no extra build, right in your browser
tags: [Facebook Login, Android key hash, SHA-1, Keystore, Release key hash, Android developer tools, Web tool]
website: https://p32929.github.io/Sha1ToMd5/
source: https://github.com/p32929/Sha1ToMd5

platforms:
  Web: https://p32929.github.io/Sha1ToMd5/
---

> **An old tool.** Made in 2019 and kept as it was.

Sha1ToMd5 gives you the key hash that Facebook Login asks for when you add an Android app. Facebook wants a short code made from your app's signing key, and the usual way to get it is to add logging code to your app, build it, run it and read the log. With this tool you skip all of that: paste the SHA-1 of your keystore and the key hash appears right away, ready to copy.

1. **Paste the SHA-1,** the colon-separated value from `keytool -list -v`, Gradle's `signingReport` or the Play Console's app signing page.
2. **Get the key hash instantly.** It is the SHA-1 bytes in base64 (for example `Xo8WBi6jzSxKDVR4drqm84yr9iU=`), which is what Facebook's "Key Hashes" field wants. The page calls it MD5.
3. **Copy it with one tap** and paste it into your Facebook app settings.
4. **Works for your release key too,** including the key Google Play signs your app with, which you can't log from a debug build.
5. **Runs in your browser.** Nothing is uploaded, and it works on phones too.

Great for Android developers adding Facebook Login who just want the key hash and move on.

I made it because I needed an easy way to get this value for Facebook Login. Every other way meant adding a log inside the Android app and running it, which took too long, so I wanted something easier.

Want the boring parts of your Android setup done for you? Contact me through my portfolio: https://p32929.github.io
