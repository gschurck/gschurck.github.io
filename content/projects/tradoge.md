---
title: "TraDOGE: Crypto trading bot with Twitter"
# weight: 1
# aliases: ["/first"]
tags: ["projects","python", "cryptocurrency"]
author: "Me"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: true
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
weight: 2
cover:
    image: "/tradoge2.png" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

# Bot de trading

DOGE trading bot for instantly buying and selling DOGE cryptocurrency on Binance when Elon Musk tweets about it.

[Github Repository](https://github.com/gschurck/tradoge)

![Screenshot](/tradoge.png)

## Technologies

- Python
- CCXT API Crypto
- Twitter API
- Websocket

## Features

- Auto trigger on new tweet with websocket
- Healthcheck to alert on downtime
- Friendly terminal UI
