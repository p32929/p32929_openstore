---
title: Office About
icon: screenshots/office-about/icon.svg
screenshots:
  - screenshots/office-about/v2-1.png
  - screenshots/office-about/v2-2.png
  - screenshots/office-about/v2-3.png
category: Developer Tools
summary: Android About Us screen library for teams. Show your company, links and team members from one JSON file, and update them without a new release
tags: [About screen, About us page, Team page, Android library, Company profile, Kotlin, JitPack, Open source]
website: https://github.com/p32929/OfficeAbout
source: https://github.com/p32929/OfficeAbout

platforms:
  Library: https://github.com/p32929/OfficeAbout
---

Office About is a ready-made "About us" screen for Android apps made by a team. Every app needs one, and building it again for each app is a chore. Put your company name, logo, links and team in one JSON file, and the library shows a clean About screen. Host the JSON online and you can change the team later without shipping an app update. It was revamped in 2026: rewritten in Kotlin, with a Material 3 look that follows light and dark mode, and it still works from Java.

I made it because I needed an easy way to show an About page, without building it again for every app. I wanted the same design everywhere, and I wanted it dynamic, so I could change it in one place on the server and it would update in every app.

1. **Team cards** with a photo (or initials), name, role and a Contact button.
2. **Company links** as buttons: Google Play, Facebook page and group, YouTube, GitHub and website. Empty links are hidden.
3. **JSON from a URL or a string,** for example from your app's assets.
4. **Loading and error screens** with a Try again button.
5. **Your own colours** if you want them.
6. **Small:** no image or JSON library added, Android 5.0 and newer.

Great for small studios and teams that publish several apps.

## Install

Add JitPack to your repositories, then the dependency:

```kotlin
// settings.gradle.kts
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()
        maven("https://jitpack.io")
    }
}
```

```kotlin
dependencies {
    implementation("com.github.p32929:OfficeAbout:2.0.0")
}
```

```kotlin
OfficeAboutHelper(this, "https://example.com/team.json").showAboutActivity()
```

Upgrading from 1.x? Your old JSON still works. See "Migrating from 1.x" on the GitHub page.

The older 2019 Java version is [MaterialOfficeAbout](https://openstore.pfay.workers.dev/app/p32929/material-office-about).
