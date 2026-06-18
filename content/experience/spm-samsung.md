---
title: "Senior AI Product Manager"
description: "Samsung Electronics, Seoul HQ, South Korea"
dateString: Mar 2023 - Present
draft: false
tags: ["AI", "Agentic", "LLM", "Voice AI"]
showToc: false
weight: 1
--- 
> Own product strategy for agentic task management, AI quality and evaluation, and the multilingual global rollout of Bixby / Galaxy AI across 400M+ Galaxy devices — setting technical and product direction across teams in the US, Korea, and India, with strategy and demos taken through to COO/EVP-level leadership.
>
> *Tap any item below to read the full story.*

## Agentic Platform — Galaxy S26 (2026)

<details class="exp">
<summary><strong>Samsung's first Agentic Assistant</strong> — co-led the Galaxy S26 launch; multi-step task execution across apps and the web (15% complex-task lift).</summary>
<div class="exp-body">
<p>Co-led Bixby's shift from a reactive command-executor into an autonomous agent that plans and executes multi-step requests. The platform is a multi-agent system: a supervisor agent orchestrates 35 specialized domain agents over a LoRA fine-tuned LLM, planning a sequence of actions and chaining them to complete a complex request end-to-end across apps and the web.</p>
<p>Shipped on the Galaxy S26 (2026), lifting complex-task completion by 15%.</p>
</div>
</details>

<details class="exp">
<summary><strong>Coverage &amp; Reliability</strong> — expanded coverage ~75% and cut the failure rate from 25% to ~6%.</summary>
<div class="exp-body">
<p>Owned the recovery layer no single team owned — the "unhappy path." For low-confidence intents, a <strong>Disambiguation Agent</strong> uses contextual cues to predict what the user actually meant and reduce conversational friction. For genuinely out-of-scope queries, a Perplexity-backed <strong>Unsupported Agent</strong> provides a graceful fallback instead of a dead end.</p>
<p>Together these expanded product coverage by roughly 75% and cut the overall failure rate from 25% to about 6%.</p>
</div>
</details>

<details class="exp">
<summary><strong>"Second Brain" (Comprehensive Answer)</strong> — on-device RAG over personal data; ~35% of complex recall queries handled within six months.</summary>
<div class="exp-body">
<p>Voice assistants were "digital amnesiacs" — great at "set a timer," useless at "what was that restaurant my friend recommended in our chat last week?" I championed a <strong>"Second Brain"</strong> vision: a personal intelligence layer that sits securely over the user's own data.</p>
<p>The Comprehensive Answer agent uses on-device Retrieval-Augmented Generation — retrieving relevant snippets from Messages, Notes, and Calendar, then synthesizing them with an LLM into a single, human-like answer. I made 100% on-device processing a non-negotiable requirement so personal data never leaves the phone.</p>
<p>It handled 25%+ of queries that previously failed with "No Answer Found," reached 35% monthly adoption within six months, and validated the broader Second Brain roadmap.</p>
</div>
</details>

## Quality &amp; Architecture

<details class="exp">
<summary><strong>LLM Evaluation Standard</strong> — 7-point binary pass/fail framework; quality 5.3 → 6.7/7 in a quarter; adopted company-wide.</summary>
<div class="exp-body">
<p>Quality was measured on a subjective 1–5 "naturalness" scale that every tester read differently, turning weekly quality reviews into opinion battles. I invented a 7-point, binary <strong>pass/fail</strong> framework — Accuracy, Relevance, Conciseness, Harmlessness, Coherence, Response Length, and View Correspondence — which removed the ambiguity entirely.</p>
<p>I turned it into a weekly dashboard that stack-ranked agents by objective score, drove a department-wide 6.5/7 release bar (shipping gated on quality, not dates), and routed bugs to the right team with clear feedback. A parallel test showed the binary system had ~50% lower variance between testers than the old scale.</p>
<p>Core-domain quality rose from 5.3 to 6.7/7 within a single quarter; the framework became the company-wide release standard, backed by a CI-integrated 5,000+ query benchmark for automated regression tracking.</p>
</div>
</details>

<details class="exp">
<summary><strong>Bixby Chat</strong> — rebuilt on a 3-tier LLM architecture with 9-category intent routing; 2× utterances, ~50% DAU/MAU lift; 14 languages on Galaxy S25.</summary>
<div class="exp-body">
<p>Replaced a brittle, manually-curated chat system with a modern LLM stack. I split chat into nine intent categories — greetings, emotional, brand protection, device info, emergency, general, and more — each with its own prompt strategy and response style (e.g. emotional replies don't push for follow-ups; greetings are more interactive).</p>
<p>Responses route across three tiers: an in-house LoRA-tuned model for personality, brand, and emotional bonding; a prompt-engineered Perplexity path for brand-advocacy and special cases; and general Perplexity as a fallback for open Q&amp;A and misclassifications.</p>
<p>Shipped in 14 languages on the Galaxy S25 (2025), doubling utterances per user and lifting DAU/MAU by about 50%.</p>
</div>
</details>

<details class="exp">
<summary><strong>Natural-Language Device Help (Device QnA)</strong> — RAG over product manuals; Device Settings failures 40% → under 10%; 15,000+ tickets/day deflected.</summary>
<div class="exp-body">
<p>Device Settings had a 40% task-failure rate. The team assumed speech recognition was at fault; I manually analyzed 1,000 failed utterances and found ASR was correct in 80%+ of them — the real problem was semantic: users said "turn on night mode" while the system looked for "Eye Comfort Shield."</p>
<p>I proposed a RAG system that indexes unstructured help content (manuals, tips, support queries) into a vector database and grounds the LLM's answer in the retrieved docs — chosen over fine-tuning for scalability and lower hallucination. A proof-of-concept on a single device manual answered 50 of the top 100 support questions and got the project greenlit.</p>
<p>After launch, Device Settings failures dropped from 40% to under 10%, deflecting 15,000+ Tier-1 support tickets a day.</p>
</div>
</details>

<details class="exp">
<summary><strong>Privacy &amp; Data Governance</strong> — lead privacy-by-design review for all Bixby AI features across the US, EU, and Korea.</summary>
<div class="exp-body">
<p>Partner with Legal on every release and own privacy-by-design review of personal-data handling — including biometric voice data and on-device sensor collection — across the US, EU, and Korea.</p>
</div>
</details>

## Leadership
- Set the agentic platform roadmap and quarterly reprioritization through to executive sign-off; authored AI-strategy briefings for COO/EVP leadership.
- Cut cross-geo dependency resolution from 7 days to under 36 hours across US, Korea, and India teams, aligning 80 PRDs into a single launch strategy.
- Mentor 4 product managers across Bangalore and Mountain View, serving as the HQ decision point for the US and India teams.
