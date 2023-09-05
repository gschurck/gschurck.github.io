---
title: "🔎 Trouve Ton Meme"
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
summary: "A powerful meme search engine"
subtitle: "A powerful meme search engine"
description: "A powerful meme search engine"
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
weight: 1
cover:
    image: "/trouve_ton_meme_hero.webp"
    alt: "Trouve Ton Meme screenshot"
    hidden: true
    responsiveImages: true
---

A website to find memes to use in chats according to:

- Categories
- Search by describing the image you are looking for

> Still in development, images are random examples currently.

[Website link](https://trouvetonmeme.com)

![Screenshot](/trouve_ton_meme.webp)

## Technologies

- Python
- Django
- HTMX for components with Ajax requests refresh without full page reload
- S3 storage for media files
- Redis cache
- CLIP AI model for image search by using image and text embeddings
- PostgreSQL database (with pgvector extension)

## Features

- Listing memes by category
- Full text search across all memes with hidden detailed description
- User accounts
- Bookmarking
- Upload meme
- Admin meme validation and moderation
- User ranking
- Rate limiting

![Diagram](/ttm-diagram.png)