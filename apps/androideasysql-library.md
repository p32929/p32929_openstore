---
title: AndroidEasySQL-Library
icon: screenshots/androideasysql-library/icon.svg
screenshots:
  - screenshots/androideasysql-library/v2-1.png
  - screenshots/androideasysql-library/v2-2.png
category: Developer Tools
summary: Android SQLite library. Create a table and add, read, update and delete rows in a few chained calls, with no SQL or SQLiteOpenHelper to write
tags: [Android SQLite, SQLite library, Android database, Kotlin, Java, JitPack, Android library, Open source]
website: https://github.com/p32929/AndroidEasySQL-Library
source: https://github.com/p32929/AndroidEasySQL-Library

platforms:
  Library: https://github.com/p32929/AndroidEasySQL-Library
---

AndroidEasySQL-Library is a small SQLite library for Android apps that just need to save data. Writing a SQLiteOpenHelper and SQL queries by hand is slow and easy to get wrong. Here you describe your columns once, and then add, read, update and delete rows with short chained calls. It was revamped in 2026: rewritten in Kotlin, with a Material 3 look that follows light and dark mode, and it still works from Java.

I made it because I was really bad at SQL. Every time I worked with SQL, I ended up building something like this, which is why I made one for Android and one for Flutter. Android apps don't need complex SQL, so as long as I could do my things properly, I was happy with it.

1. **No SQL to write:** describe the columns once and the table is built for you.
2. **An ID column for free:** every table gets an auto-increment primary key.
3. **Chained calls:** add or update a whole row in one line.
4. **Read rows as a simple list,** or as a Cursor if you prefer, ordered by any column.
5. **Search, count and match** values across columns.
6. **Store text, numbers, Long and Double values,** or null.
7. **Tiny:** no extra dependencies, Android 5.0 and newer.

The sample app in the repo is a small notes app built with it. Great for small Android apps that need a local database without the boilerplate.

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
    implementation("com.github.p32929:AndroidEasySQL-Library:2.0.0")
}
```

```kotlin
val db = EasyDB.init(context, "Notes")
    .setTableName("Notes")
    .addColumn("Title", "text", "not null")
    .addColumn("Body", "text")
    .doneTableColumn()

db.addData("Title", "Groceries").addData("Body", "Milk and eggs").doneDataAdding()
val notes = db.getAllRows()
```

Upgrading from 1.x? Most code works as is. See "Migrating from 1.x" on the GitHub page.

Want a database set up for your Android app without the SQL headache? Contact me through my portfolio: https://p32929.github.io
