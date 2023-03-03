---
title: "Trouve Ton Meme: Meme finder website"
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
description: "Don't lose time searching for a meme"
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
weight: 3
cover:
    image: "/trouve_ton_meme.png" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
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
