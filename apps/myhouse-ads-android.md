---
title: MyHouse Ads Android
icon: screenshots/myhouse-ads-android/icon.svg
screenshots:
  - screenshots/myhouse-ads-android/shot-1.png
  - screenshots/myhouse-ads-android/shot-2.png
  - screenshots/myhouse-ads-android/shot-3.png
category: Developer Tools
summary: Android house ads library. Promote your own apps inside your other apps with banner and interstitial ads, with no ad network
tags: [House ads, Cross promotion, Android ads, Banner ads, Interstitial ads, Android library, Java, JitPack]
website: https://github.com/p32929/MyHouseAdsAndroid
source: https://github.com/p32929/MyHouseAdsAndroid

platforms:
  Library: https://github.com/p32929/MyHouseAdsAndroid
---

MyHouse Ads Android is a library for showing house ads: ads for your own apps, inside your own apps. If you have a few apps, the people using one are the easiest to bring to the next, and you don't need an ad network or a revenue share to do it. List your apps in a JSON file or in code, and the library shows them as banners and full-screen ads.

1. **Banner and interstitial ads** with your app icons, names and Play Store links.
2. **Two ways to add ads:** a JSON file you host, or a list right in your code.
3. **Show an ad on back press** with one override. If there is nothing to show, back works as usual.
4. **No third-party ad SDK** and no revenue share.

Great for developers with several apps who want to cross-promote them for free. A newer version with a rating dialog is [House Ads 2](https://github.com/p32929/HouseAds2).

## Install

Add JitPack to your root `build.gradle`, then the dependency:

```gradle
allprojects { repositories { maven { url 'https://jitpack.io' } } }

dependencies {
    implementation 'com.github.p32929:MyHouseAdsAndroid:1.0.2'
}
```
