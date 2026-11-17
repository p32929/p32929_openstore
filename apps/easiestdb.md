---
title: EasiestDB
icon: screenshots/easiestdb/icon.png
screenshots:
  - screenshots/easiestdb/1.png
category: Developer Tools
summary: The easiest way to use a SQLite database in Flutter. Declare your tables once, then add, read, search, update and delete without writing SQL
tags: [Flutter, SQLite, Flutter database, sqflite, Dart, CRUD, pub.dev, Mobile development]
website: https://github.com/p32929/EasiestdbFlutter
source: https://github.com/p32929/EasiestdbFlutter

platforms:
  Library: https://pub.dev/packages/easiestdb
---

EasiestDB is the easiest way to use a SQLite database in a Flutter app. Writing SQL queries by hand for every table is slow and easy to get wrong. With EasiestDB you list your tables and columns once, and then add, read, search, update and delete rows with simple calls, without writing a single query.

I made it because I was really bad at SQL. Every time I worked with SQL, I ended up building something like this, which is why I made one for Android and one for Flutter. Android apps don't need complex SQL, so as long as I could do my things properly, I was happy with it.

1. **Set up in a few lines:** name the database, its tables and their columns. An ID column is added for you.
2. **All the basics:** add data, get all rows or one row, search by a column, update by ID and delete.
3. **Column rules:** add SQL constraints like `UNIQUE` to any column.
4. **Raw SQL when you need it:** it uses `sqflite` underneath, so you can still run your own queries.

Great for Flutter apps that need a simple local database.

This is an older package and is marked as discontinued on pub.dev.

## Install

```bash
flutter pub add easiestdb
```

Want a custom version of this app, or help changing it for your needs? Contact me through my portfolio: https://p32929.github.io
