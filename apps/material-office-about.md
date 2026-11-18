---
title: MaterialOfficeAbout
icon: screenshots/material-office-about/icon.svg
screenshots:
  - screenshots/material-office-about/shot-1.png
  - screenshots/material-office-about/shot-2.png
category: Developer Tools
kind: personal
summary: Older Java version of Office About. A Material Design About Us screen for Android team apps, loaded from one JSON file you host
tags: [About screen, About us page, Team page, Android library, Material Design, Java, JitPack, Open source]
website: https://github.com/p32929/MaterialOfficeAbout
source: https://github.com/p32929/MaterialOfficeAbout

platforms:
  Library: https://github.com/p32929/MaterialOfficeAbout
---

> **An older version.** This is the 2019 Java version. [Office About](https://openstore.pfay.workers.dev/app/p32929/office-about) 2.0.0 is the newer one, rewritten in 2026 in Kotlin with Material 3 and light and dark mode, using the same kind of JSON file. This library is kept as it was.

MaterialOfficeAbout is a ready-made Material Design "About us" screen for Android apps made by a team. Every app needs one, and building it again for each app is a chore. Put your company logo, social links and team members in one JSON file you host, and the library shows them in a clean About screen. Change the file, and every app shows the new team, with no new release.

I made it because I needed an easy way to show an About page, without building it again for every app. I wanted the same design everywhere, and I wanted it dynamic, so I could change it in one place on the server and it would update in every app.

What makes it different: two lines of code add the whole screen, and all the content comes from your JSON file, so nobody has to touch the app to update the team.

1. **A Material Design About screen** with your logo, social links and team members.
2. **Team details from a JSON file,** so you update the team without shipping a new build.
3. **Toolbar on or off,** your choice.
4. **Add your own views** to the screen with a `LoadListener`.
5. **Shuffle the member list** but keep one person at the top, by name or by role.
6. **Free and open source.**

Great for teams and small companies that publish several Android apps and want the same About screen in all of them.

How to use it: add JitPack to your repositories and `implementation 'com.github.p32929:MaterialOfficeAbout:1.0.6'` to your dependencies. Then create `new OfficeAboutHelper(this, "your JSON link")` and call `showAboutActivity()`. If you use ProGuard, add the keep rule from the README. For new apps, Office About 2.0.0 is the better choice.

Want a clean About screen for your team's apps? Contact me through my portfolio: https://p32929.github.io
