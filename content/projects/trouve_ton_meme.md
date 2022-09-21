---
title: "Trouve Ton Meme"
# weight: 1
# aliases: ["/first"]
tags: ["projects"]
#author: "Me"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "Crypto Twitter trading bot"
canonicalURL: "https://canonical.url/to/page"
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
weight: 1
cover:
    image: "/trouve_ton_meme.png" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
editPost:
    URL: "https://github.com/<path_to_repo>/content"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---

# Bot de trading

![Screenshot](/trouve_ton_meme.png)

## Technologies

- Python
- Django
- Django-Unicorn for components with Ajax requests refresh without page reload
- S3 storage for media files

## Features

- Listing memes by category
- Full text search across all memes with hidden detailed description
- User accounts
- Bookmarking
- Upload meme
- Admin meme validation
- User ranking
- Rate limiting
