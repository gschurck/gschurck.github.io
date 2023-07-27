---
title: "🐋 Lightwhale: Docker memory optimizer on Linux"
# weight: 1
# aliases: ["/first"]
tags: ["projects"]
author: "Me"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: true
comments: false
summary: "Free up memory taken by your unused Docker containers"
description: "Free up memory taken by your unused Docker containers"
canonicalURL: "https://gschurck.github.io/projects/lightwhale/"
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
weight: 2
cover:
    image: "/lightwhale.png"
    hidden: false
---

## Intro

Often you'll have a lot of Docker containers running on your computer or server, and you don't really use them much. So they are still running and taking up precious memory.

Okay, but wait, if we shut down these containers to free up memory, we have to start them up again later. That takes time and it's not very convenient or optimal.

It would be really cool if we could free up that memory while keeping the containers accessible and ready to use when we need them, right?

That's why I wanted to create this tool.

Lightwhale can automatically save the memory state of containers that have not been used for a while, and instantly restore them when a request reaches them.

> This project is still in work in progress, I will open source it once it's ready.

## Video demonstration

Demonstration of a prototype using a custom Go proxy and Linux iptables.

{{< youtube miGcR-hPLTI >}}

## Architecture

Lightwhale automatically saves the memory state of containers that have not been used for a while and stops them.

By routing all container requests through a proxy, Lightwhale can hold a request (to what is essentially a non-existent container), restore the container with its memory state, and then pass the request through.

It uses [Docker checkpoints](https://docs.docker.com/engine/reference/commandline/checkpoint/) under the hood to save and restore memory state of containers.

The tool can also track all new containers to automatically add them to its database and route requests to new container ports through the proxy using iptables.

### Architecture diagram

> You can zoom in on the diagram by clicking on it

![](/lightwhale-mermaid-diagram.svg)

## Technologies

- Linux
- Docker
- Go
- Proxy
- Iptables

## Limitations

- Because Lightwhale uses incoming requests to guess when a container is not in use and to trigger the restoration of the container, it can't work with containers running long-running processes or cron jobs.
- Another not-insignificant issue I've come across is that communication between containers does not go through the host's iptables and the custom lightwhale proxy, but directly through a Docker network. This is indeed an important issue, as it could be really useful for a project using a huge docker compose, for example. I am still investigating to find an effective solution to deal with this.