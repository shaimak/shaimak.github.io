---
title: "HomeLab"
description: "My Self-hosted Services"
draft: false
tags: ["AI", "Self-hosting"]
showToc: false
weight: 1
cover:
    image: "projects/homelab/stack.png#center"
--- 
> A homelab is a personal server I run at home to host my own services, experiment, and learn.

I first tried **CasaOS** (the dashboard above). It is an app-store style layer that makes self-hosting almost one-click, so it was an easy way in. As I ran more, I wanted something lighter and more robust: fully reproducible, properly reverse-proxied, and behind a single login. So I rebuilt everything as a hand-managed **Docker Compose + Caddy** stack. It runs leaner, survives reboots and moves cleanly between machines, and I control every moving part.

### What I run now
Every service sits behind one reverse proxy, with automatic HTTPS and a single sign-on:

- **Caddy**: reverse proxy that terminates HTTPS and routes each subdomain to a container. Certificates issue and renew on their own.
- **Authentik**: single sign-on. One account logs me into every service over OIDC.
- **Outline**: my wiki and knowledge base.
- **Guacamole**: my desktop in the browser (RDP / VNC / SSH), reachable from anywhere.
- **Paperless-ngx**: scanned documents, OCR'd and searchable.
- **ddclient**: keeps my domain pointed at my home IP as it changes, via Porkbun DNS.
- **vnstat**: bandwidth accounting for the connection.

On top of this stack I also run **Ravi**, a self-hosted AI assistant I reach over Telegram and the web. [More on Ravi here.](/projects/ravi/)

### Why self-host
- I own the data. It lives on my disk, not someone else's server.
- Privacy. Nothing leaves my hardware.
- It is a real exercise in networking, DNS, TLS, containers, and single sign-on.
- The whole stack is portable. Moving to a new machine is copying the repo, the data, and the secrets, then bringing it back up.

### Open-source starter kit
I packaged the infrastructure into a reusable kit so anyone can stand up the same thing. It has every compose file, per-service setup guides, and the gotchas I hit along the way.

**GitHub: [shaimak/docker-startup-kit](https://github.com/shaimak/docker-startup-kit)**
