---
title: House Ads 2
icon: screenshots/house-ads-2/icon.svg
screenshots:
  - screenshots/house-ads-2/shot-1.jpg
  - screenshots/house-ads-2/shot-2.jpg
  - screenshots/house-ads-2/shot-3.jpg
category: Developer Tools
summary: Android house ads library. Cross-promote your own apps with banner and interstitial ads from a JSON file you host, plus a rating dialog
tags: [House ads, Cross promotion, Android ads, Banner ads, Interstitial ads, Rating dialog, Android library, JitPack]
website: https://github.com/p32929/HouseAds2
source: https://github.com/p32929/HouseAds2

platforms:
  Library: https://github.com/p32929/HouseAds2
---

House Ads 2 is an Android library for promoting your own apps inside your other apps, with banner and full-screen ads. Ad networks take a cut and track your users. Here the ads come from a JSON file you host yourself, so you can change them any time without shipping an app update.

1. **Banner and interstitial ads** for your own apps, from your own JSON file.
2. **Change ads without an update:** edit the JSON and every install picks it up.
3. **Rotating banners** that change every few seconds, on a timer you set.
4. **Rating dialog:** it asks unhappy users for feedback by email before sending happy ones to the Play Store.
5. **No ad network,** no revenue share and no tracking.

Great for developers with several apps who want free cross-promotion and better Play Store ratings.

## Install

Add JitPack to your root `build.gradle`, then the dependency:

```gradle
allprojects { repositories { maven { url 'https://jitpack.io' } } }

dependencies {
    implementation 'com.github.p32929:HouseAds2:1.0.0.16'
}
```
