---
title: House Ads 2
icon: screenshots/house-ads-2/icon.svg
screenshots:
  - screenshots/house-ads-2/v2-1.png
  - screenshots/house-ads-2/v2-2.png
  - screenshots/house-ads-2/v2-3.png
category: Developer Tools
kind: personal
summary: Android house ads library. Cross-promote your own apps with a banner, a full-screen app list and a rating dialog, from a JSON file you host
tags: [House ads, Cross promotion, Android ads, Banner ads, Interstitial ads, Rating dialog, Android library, Kotlin, JitPack]
website: https://github.com/p32929/HouseAds2
source: https://github.com/p32929/HouseAds2

platforms:
  Library: https://github.com/p32929/HouseAds2
---

House Ads 2 is an Android library for promoting your own apps inside your other apps. Ad networks take a cut and track your users. Here the ads come from a JSON file you host yourself, so you can change them any time without shipping an app update, with no ad network, no tracking and no revenue share. It was revamped in 2026: rewritten in Kotlin, with a Material 3 look that follows light and dark mode, and it still works from Java.

I made it because paying for ads was expensive, and I had a lot of apps at that time. So I thought: why not promote my own apps inside my own apps?

1. **Banner ad** for one of your apps, with its icon, name, description and a Get button.
2. **Full-screen list of all your apps,** with Share, Rate and Exit buttons. A good fit for the back button.
3. **Rating dialog** that sends 5-star users to the Play Store and asks everyone else for feedback by email.
4. **Rotating banners** that switch to the next app on a timer you choose.
5. **Change the ads without an update:** edit the JSON and every install picks it up.
6. **Follows your app's look,** and hides the app that is showing the ads.

Great for developers with several apps who want free cross-promotion and better Play Store ratings.

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
    implementation("com.github.p32929:HouseAds2:2.0.0")
}
```

```kotlin
val houseAds = HouseAds(this, "https://your.site/ads.json", findViewById(R.id.adsLl))
houseAds.autoChangeBannerAds(60)            // next app every 60 seconds
houseAds.setFeedbackEmail("you@example.com") // turns on the rating dialog
onBackPressedDispatcher.addCallback(this) { houseAds.showInterAds() }
```

Upgrading from 1.x? The main calls are the same, so most apps only need the new version number.

Have a few apps and want them to help each other grow? Contact me through my portfolio: https://p32929.github.io
