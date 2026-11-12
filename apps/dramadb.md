---
title: DramaDB
icon: screenshots/dramadb/icon.png
screenshots:
  - screenshots/dramadb/1.png
  - screenshots/dramadb/2.png
  - screenshots/dramadb/3.png
category: Entertainment
summary: Find the good Korean and Asian dramas using ratings, reviews and comments, with filters the original site never had
tags: [Korean drama, Asian drama, TV series, Ratings, Filters, Web scraping, Personal project]

platforms:
  Web: https://raw.githubusercontent.com/p32929/p32929_openstore/main/unavailable.png
---

I love watching Korean dramas, but I could never tell the good ones from the bad ones. The site I watched on, KissAsian, had thousands of dramas and almost no way to filter them. There was no easy way to see which ones people actually liked, so I wasted a lot of time on dramas that turned out to be bad.

**So I built DramaDB for myself.** I scraped KissAsian with an automated browser, collecting each drama's country, genre, year, status, episode count, views, ratings, reviews and comments. Then I made a Next.js website from that data and hosted it on Vercel. Now I pick a drama by what viewers say about it, not just by its name or its poster.

You can filter by country, genre, status, year and number of episodes. You can sort by rating, by review score, by number of comments, by number of reviewers or by views, so the dramas people loved come first. Every drama shows its poster, and it works on desktop and on a phone.

This was a personal project, made to solve my own problem. It uses no server, so the whole list loads in the browser.
