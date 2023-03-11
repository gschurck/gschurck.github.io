---
title: "🔎 Trouve Ton Meme: Meme finder website"
# weight: 1
# aliases: ["/first"]
tags: ["projects", "python", "django"]
author: "Me"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: true
comments: false
summary: "Stop wasting time searching for memes"
description: "Stop wasting time searching for memes"
canonicalURL: "https://canonical.url/to/page"
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: false
ShowRssButtonInSectionTermList: true
UseHugoToc: true
weight: 4
---

A website to find memes to use in chats according to:

- Categories
- Search by describing the image you are looking for

> Still in development, images are random examples currently.

[Website link (will be up again soon)](https://jsklgnvatw.eu07.qoddiapp.com)

![Screenshot](/trouve_ton_meme.png)

## Technologies

- Python
- Django
- Django-Unicorn for components with Ajax requests refresh without page reload
- S3 storage for media files
- Redis cache

## Features

- Listing memes by category
- Full text search across all memes with hidden detailed description
- User accounts
- Bookmarking
- Upload meme
- Admin meme validation
- User ranking
- Rate limiting
