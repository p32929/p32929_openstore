---
title: MyHouse Ads Android
icon: screenshots/myhouse-ads-android/icon.svg
screenshots:
  - screenshots/myhouse-ads-android/v2-1.png
  - screenshots/myhouse-ads-android/v2-2.png
category: Developer Tools
kind: personal
summary: Android house ads library. Promote your own apps inside your other apps with a banner and an interstitial, with no ad network or revenue share
tags: [House ads, Cross promotion, Android ads, Banner ads, Interstitial ads, Android library, Kotlin, JitPack]
website: https://github.com/p32929/MyHouseAdsAndroid
source: https://github.com/p32929/MyHouseAdsAndroid

platforms:
  Library: https://github.com/p32929/MyHouseAdsAndroid
---

MyHouse Ads Android shows house ads: ads for your own apps, inside your own apps. If you have a few apps, the people using one are the easiest to bring to the next, and you don't need an ad network, an account or a revenue share to do it. List your apps in a JSON file you host or right in your code, and the library shows them as a banner and a full-screen ad. It was revamped in 2026: rewritten in Kotlin, with a Material 3 look that follows light and dark mode, and it still works from Java.

I made it because paying for ads was expensive, and I had a lot of apps at that time. So I thought: why not promote my own apps inside my own apps?

1. **Banner ad** with your app's icon, a short line of text and a Get button.
2. **Interstitial ad:** a centered card with a big icon, Get it and Later.
3. **Ad on back press:** the close button says Exit, so the ad never traps your users.
4. **Every app gets its turn:** each time an ad shows, the next app in your list is used.
5. **Two ways to feed it:** a JSON file at any URL, or a list in code.
6. **Small:** no image or network library is added to your app.

Great for developers with several apps who want to cross-promote them for free. For rotating banners and a rating dialog too, see House Ads 2.

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
    implementation("com.github.p32929:MyHouseAdsAndroid:2.0.0")
}
```

```kotlin
// The banner goes into this LinearLayout
val ads = MyAdsAdder(this, linearLayout, "https://example.com/house_ads.json")

// Show an interstitial anywhere
ads.showInterAd(this, false)
```

Upgrading from 1.x? The class and method names are the same, so most apps only need the new version number.

Have a few apps and want them to help each other grow? Contact me through my portfolio: https://p32929.github.io
