---
title: Office About
icon: screenshots/office-about/icon.svg
screenshots:
  - screenshots/office-about/shot-1.png
category: Developer Tools
summary: Android About Us screen library for teams. Show your company logo, links and team members from a JSON file, in two lines of code
tags: [About screen, About us page, Android library, Team page, Company profile, Java, JitPack, Open source]
website: https://github.com/p32929/OfficeAbout
source: https://github.com/p32929/OfficeAbout

platforms:
  Library: https://github.com/p32929/OfficeAbout
---

Office About is a ready-made "About us" screen for Android apps built by a team. Every app needs one, and it is boring to build again and again. Put your company logo, links and team members in a JSON file, and the library shows a clean About screen in two lines of code. Change the team later by editing the JSON, with no app update.

1. **Company logo and links:** Play Store, Facebook page and group, YouTube, GitHub and website.
2. **Team list** with a photo, name, role and contact link for each person.
3. **Update without a new release:** edit the JSON and every install shows the change.
4. **Two lines to add:** create the helper and call `showAboutActivity()`.

Great for small studios and teams that publish several apps. A newer version is [MaterialOfficeAbout](https://github.com/p32929/MaterialOfficeAbout).

## Install

Add JitPack to your root `build.gradle`, then the dependency:

```gradle
allprojects { repositories { maven { url 'https://jitpack.io' } } }

dependencies {
    implementation 'com.github.p32929:OfficeAbout:1.0.0.7'
}
```
