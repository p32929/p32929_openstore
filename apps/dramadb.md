---
title: DramaDB
icon: screenshots/dramadb/icon.png
screenshots:
  - screenshots/dramadb/1.png
  - screenshots/dramadb/2.png
  - screenshots/dramadb/3.png
category: Entertainment
summary: Thousands of Korean dramas and no way to tell the good ones. DramaDB lets you filter and sort by ratings, reviews and comments, so the loved ones come first
tags: [Korean drama, Asian drama, TV series, Ratings, Filters, Web scraping, Personal project]

platforms:
  Web: https://raw.githubusercontent.com/p32929/p32929_openstore/main/unavailable.png
---

**Stop wasting evenings on bad dramas. DramaDB shows you which Korean and Asian dramas people actually loved.**

## The problem

I love watching Korean dramas, but I could never tell the good ones from the bad ones. The site I watched on, KissAsian, had thousands of dramas and almost no way to filter them. There was no easy way to see which ones people actually liked, so I wasted a lot of time on dramas that turned out to be bad.

## How DramaDB solves it

I collected every drama's details, ratings, reviews and comments, and put them on one page you can filter and sort. Now I pick a drama by what viewers say about it, not just by its name or its poster.

1. **Filter** by country, genre, status, year and number of episodes.
2. **Sort** by rating, review score, number of comments, number of reviewers or views, so the dramas people loved come first.
3. **Every drama shows its poster**, and it works on desktop and on a phone.

## How I built it

I scraped KissAsian with an automated browser, collecting each drama's country, genre, year, status, episode count, views, ratings, reviews and comments. Then I made a Next.js website from that data and hosted it on Vercel. It uses no server, so the whole list loads in the browser. This was a personal project, made to solve my own problem.
