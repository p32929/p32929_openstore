---
title: AndroidEasySQL-Library
icon: screenshots/androideasysql-library/icon.svg
screenshots:
  - screenshots/androideasysql-library/1.png
category: Developer Tools
summary: Android SQLite library that lets you create tables, add, read, search, update and delete data in a few chained lines, with no SQL to write
tags: [Android SQLite, SQLite library, Android database, SQLiteOpenHelper, Java, JitPack, Android library, Open source]
website: https://github.com/p32929/AndroidEasySQL-Library
source: https://github.com/p32929/AndroidEasySQL-Library

platforms:
  Library: https://github.com/p32929/AndroidEasySQL-Library
---

AndroidEasySQL-Library is an Android SQLite library for people who just want to save data, not write a SQLiteOpenHelper and SQL queries by hand. You set up the database and its columns in one chained call, then add, read, search, update and delete rows with short, readable methods.

1. **Set up in one go:** name the database and table, and add columns with "unique" or "not null" rules, all in one chain.
2. **No primary key to manage:** an ID column is added for you.
3. **Add data** by column number or column name.
4. **Read data** as a Cursor, all rows or ordered by any column.
5. **Search** one row, or match values across several columns.
6. **Update and delete** single rows, or clear the whole table.

Great for small Android apps that need a local database without the usual boilerplate. A newer version (V2) lives at [EasiestSqlLibrary](https://github.com/p32929/EasiestSqlLibrary), and there is a Flutter version called [EasiestDB](https://pub.dev/packages/easiestdb).

## Install

Add JitPack to your root `build.gradle`, then the dependency:

```gradle
allprojects { repositories { maven { url 'https://jitpack.io' } } }

dependencies {
    implementation 'com.github.p32929:AndroidEasySQL-Library:1.4.1'
}
```
