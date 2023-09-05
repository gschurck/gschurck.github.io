---
title: "🔎 Software Finder"
# weight: 1
# aliases: ["/first"]
tags: ["projects","graph","neo4j","svelte", "sveltekit", "typescript", "serverless", "vercel"]
showToc: true
TocOpen: false
draft: false
hidemeta: true
comments: false
summary: "A new way to find software alternatives using knowledge graph"
description: "A new way to find software alternatives knowledge graph"
canonicalURL: "https://gschurck.github.io/projects/software-finder/"
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
weight: 3
cover:
    image: "/software-finder.webp" # image path/url
    alt: "Software Finder screenshot" # alt text
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
    responsiveImages: true
# A website of softwares similarities
---

## Intro

The goal of this project is to find software alternatives without even specifying each different functionality.

We are used to search on Google the details of the features to maybe desperately find the software of our dreams.
But Google is not very good at it.

So I wanted to use a different way of finding things.
With this tool, no more need to detail specific features.
Just enter 2 softwares of which you would like to find an alternative, and you will get a mixture of both.

[Project link](https://software-graph.vercel.app)

![](/software-finder.webp)

## Under the hood

- Softwares are saved in a Neo4j graph database
- Each software is linked in with softwares that have the closer features
- Which ends with a knowledge graph of softwares similarity
- Results are a shortest path query sorted according to the level of similarity, from one software to the other.

![Graph](/bloom-visualisation-cropped.webp)

## Technologies

- Neo4j
- Sveltekit
- TypeScript
- Serverless
- TailwindCSS

## Features

- Select 2 softwares
- Get the list of all alternatives which have similar features of both softwares.
  ![](/software-merger.webp)
- Explore the graph of the whole software ecosystem
  ![](/software-graph.webp)

## Issues

### Data

It will become very difficult to collect data manually and categorize it accurately at a larger scale.

And unfortunelately, I don't know any AI that would be capable of doing this kind of work by itself...
Indeed, this kind of data need precision for the project to stay reliable.
