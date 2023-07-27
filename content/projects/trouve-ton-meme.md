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
canonicalURL: "https://gschurck.github.io/projects/trouve-ton-meme/"
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
weight: 3
cover:
    image: "/trouve_ton_meme_hero.png"
    hidden: true
---

A website to find memes to use in chats according to:

- Categories
- Search by describing the image you are looking for

> Still in development, images are random examples currently.

[Website link](https://dev.trouvetonmeme.com)

![Screenshot](/trouve_ton_meme.png)

## Technologies

- Python
- Django
- HTMX for components with Ajax requests refresh without full page reload
- S3 storage for media files
- Redis cache
- BLIP AI model for image description generation
- PostgreSQL database (with word trigram similarity search)

## Features

- Listing memes by category
- Full text search across all memes with hidden detailed description
- User accounts
- Bookmarking
- Upload meme
- Admin meme validation and moderation
- User ranking
- Rate limiting
