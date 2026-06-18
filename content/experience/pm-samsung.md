---
title: "AI Product Manager"
description: "Samsung Electronics, Seoul HQ, South Korea"
dateString: Aug 2019 - Feb 2023
draft: false
tags: ["AI", "ML", "Voice AI", "On-Device"]
showToc: false
weight: 2
--- 
> Drove user growth and on-device innovation on Bixby, scaling the platform from 150M to 300M+ users and owning the end-to-end lifecycle for flagship AI features reaching tens of millions.
>
> *Tap any item below to read the full story.*

## On-Device AI

<details class="exp">
<summary><strong>On-Device Bixby (Founding PM)</strong> — scoped Samsung's first on-device assistant; 35% server-cost savings, ~30% faster, 90%+ adoption. "Best Feature in AI Team" (2021).</summary>
<div class="exp-body">
<p>The vision was to run Bixby entirely on-device for speed, privacy, and offline use — but a lift-and-shift of 3,000+ server-side goals was impossible on a phone. As founding PM, I scoped an impossible vision into a shippable V1 through three judgment calls:</p>
<p>(1) <strong>NLU</strong> — usage data showed 20 core goals (alarms, flashlight, and the like) covered 50% of all Bixby usage, so I de-scoped the model to just those, sacrificing the long tail to make it feasible. (2) <strong>ASR</strong> — non-negotiable quality, allocating the size budget for a 200MB model at 99% accuracy. (3) <strong>TTS</strong> — pre-load only the single default brand voice that most users actually used.</p>
<p>Shipped on the Galaxy Z Flip (2021): 90%+ adoption in the US and Korea, ~10% of global Bixby traffic handled on-device, 35% server-cost savings, and ~30% lower latency. Won "Best Feature in AI Team" (2021).</p>
</div>
</details>

## Consumer AI Features

<details class="exp">
<summary><strong>Personal Voice Creator</strong> — Samsung's first consumer voice-cloning feature; 20M users; chose privacy over speed-to-market.</summary>
<div class="exp-body">
<p>An engineer on my TTS team prototyped voice cloning from ~18 recorded sentences. The fast path was server-side processing — but voice is intensely personal biometric data, and privacy ("always listening") was already Bixby's top user complaint.</p>
<p>I advocated against the faster server approach, arguing the long-term cost of lost trust outweighed being first to market, and won a ~6-month delay to build the entire pipeline <strong>100% on-device</strong>: no voice data ever leaves the phone, zero logging, privacy by default. We launched iteratively via Bixby Labs, leading with the safest, most compelling use cases — Call Screening and Bixby personalization.</p>
<p>Reached 20M users shortly after launch, earned positive privacy-focused press, and set the on-device gold standard for sensitive-data AI features at Samsung. — <a href="https://timesofindia.indiatimes.com/gadgets-news/samsungs-bixby-can-now-be-your-new-personal-voice-clone-to-annoy-spammers/articleshow/103364266.cms">global media coverage</a></p>
</div>
</details>

<details class="exp">
<summary><strong>Text Call</strong> — on-device AI call screening; 50M+ uses; became a foundation for Galaxy AI.</summary>
<div class="exp-body">
<p>I conceived an on-device ASR feature to answer and transcribe calls for spam screening — but it depended on the Phone App team, whose goal (serve all 1B Samsung users) conflicted with mine (drive Bixby engagement via Bixby branding and registration).</p>
<p>Rather than force my goal, I created a shared one: a best-in-class, privacy-first screening feature for <em>all</em> Samsung users, with Bixby's AI as the foundational tech. I made real compromises — dropped "Bixby" from the name (just "Text Call"), de-scoped to 100% on-device ASR with a simple preset-message UI (no Bixby registration needed), and gave the Phone App team equal credit. I embedded my lead engineer with their team to co-design a secure real-time audio path.</p>
<p>Launched on time with 50M+ uses and an NPS lift of ~20 points — the first time Bixby's AI powered the whole Samsung ecosystem, and a foundation for what became <a href="https://www.samsung.com/us/support/answer/ANS00092302/">Galaxy AI</a>.</p>
</div>
</details>

<details class="exp">
<summary><strong>Bixby Labs &amp; Custom Wake-up</strong> — founded Samsung's first opt-in AI experimentation platform; Custom Wake-up hit 17% activation and 25% higher weekly actives.</summary>
<div class="exp-body">
<p><a href="https://www.phonearena.com/news/bixby-gets-major-update_id145783">Custom Wake-up</a> (name Bixby anything) was exciting but imperfect — an 8% false-reject rate versus 2% for "Hi Bixby," and only two languages. A full launch risked the brand; killing it wasted the innovation.</p>
<p>I proposed a third path: <strong>Bixby Labs</strong>, an opt-in beta platform with clear expectations, a server-side kill-switch, and built-in data collection — letting us ship quickly but safely and learn from enthusiastic early adopters. I had to win a backbone debate with the Head of QA, who opposed shipping anything below the quality bar; I argued that for novel AI, a controlled real-user release is the only way to <em>reach</em> the bar.</p>
<p>Custom Wake-up hit 17% activation and 25% higher weekly actives vs. control, with positive press — and Bixby Labs is now the org's standard launch-and-learn channel for all experimental AI features.</p>
</div>
</details>

<details class="exp">
<summary><strong>Voice Unlock &amp; Hands-Free</strong> — turned an "impossible" voice-unlock request into a 3-tier risk model; 40% of commands now run over the lock screen.</summary>
<div class="exp-body">
<p>The top user request was to unlock the phone by voice — but literal voice-unlock was impossible, since Android biometric policy requires 99.9% accuracy that voice can't meet. I reframed the real need: users didn't want to <em>unlock</em>, they wanted to <em>get things done</em> hands-free.</p>
<p>I categorized 100+ Bixby actions into three risk tiers — low (toggle flashlight), medium (call mom, read last message), high (delete a contact, turn off mobile data) — and designed safeguards: masking the caller number on the lock screen, a clear opt-in "use Bixby while locked" setting, and voice-match as step-up authentication for high-risk actions only.</p>
<p>Result: 40% of all Bixby commands now execute over the lock screen. I also added Continuous Conversation (on-device audio rejection, speaker verification, and a contextual turn classifier) for wake-word-free follow-ups.</p>
</div>
</details>
