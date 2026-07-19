---
title: "Ravi — My AI Assistant"
description: "A self-hosted AI assistant on my homelab"
draft: false
tags: ["AI", "Self-hosting"]
showToc: false
weight: 3
--- 
> Ravi is a self-hosted AI assistant that runs on my homelab. I talk to it from Telegram or WhatsApp, and it can act on my own tools and data.

Ravi is built on **OpenClaw**, runs entirely on my own hardware, and uses free-tier models. Because it is self-hosted, my prompts and data stay on my machine.

*This article is a work in progress. I will keep adding use cases here as I find more use for them.*

### Ask my own knowledge base
Ravi is connected to my Outline wiki, so I can ask questions over my own notes. It searches, reads, and writes pages, which means I can pull up something I wrote months ago or have Ravi draft a new page for me in plain language.

### Turn topics and books into podcasts
Ravi researches a topic, or reads a chapter from a book I drop in, and generates a two-host audio podcast. The voices use **Microsoft Edge TTS**, which is free and sounds natural. The finished episode is sent straight to me on Telegram, so I can listen on the go.

### Find cheap flights
Ravi searches live **Google Flights** data, so I can ask for the cheapest dates or routes in plain language and get real prices back. No API key, no manual searching.

### Drive the browser
Ravi can log in, fill forms, and pull information from web pages, which lets it handle multi-step tasks on the sites I use.

### Make diagrams
It generates architecture and flow diagrams from a description, useful when I want to sketch out an idea quickly.

### Remember what matters
Ravi keeps a searchable memory, so I tell it a preference once and it recalls it later.

### How I reach it
- **WhatsApp**: easy to connect and always on my phone, good for quick questions.
- **Telegram**: my preferred channel for sharing large files, since it handles the podcast audio and documents Ravi sends without the size limits.
- **Web**: a browser UI behind my single sign-on, reachable from anywhere.

Ravi runs on the same stack as the rest of my [homelab](/projects/homelab/).
