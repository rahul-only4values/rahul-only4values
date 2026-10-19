<p align="center"><img src="assets/banner.svg" alt="Rahul Soni. I build custom software for hard business problems, then test whether it worked." width="100%"></p>

<p align="center">
<a href="https://irahulsoni.com"><b>irahulsoni.com</b></a> &nbsp;·&nbsp;
<a href="https://www.linkedin.com/in/irahulsoni"><b>LinkedIn</b></a> &nbsp;·&nbsp;
<a href="https://github.com/emberyard"><b>emberyard</b></a> &nbsp;·&nbsp;
<a href="https://emberyard.github.io/idx-site/"><b>IDX</b></a>
</p>

I build custom software for hard business problems, and AI is the sharpest tool I use for it. I work as one operator with a fleet of coding agents, and I care about one thing above the rest: does it actually work. So I test my own results and write down the ones that fail.

<p align="center"><img src="assets/fleet.svg" alt="A company does five things: sense, execute, remember, report, decide. Four can be automated; deciding stays with the operator. Six layers from reality to views." width="100%"></p>

## Systems I have built

Each of these is a layered pipeline with one hard problem and one idea that cracked it. The private ones are described, not shown.

<p align="center"><img src="assets/sys-library.svg" alt="Expert-video research library: find experts, score, transcribe, index by moment, ask a question, jump to the second" width="100%"></p>
<p align="center"><img src="assets/sys-dubbing.svg" alt="AI dubbing: listen, translate, new voice, keep the music, fit the video, final cut" width="100%"></p>
<p align="center"><img src="assets/sys-docai.svg" alt="Document AI in layers: any document in, building blocks, extract, validate, a person checks, deliver" width="100%"></p>
<p align="center"><img src="assets/sys-redesign.svg" alt="Redesign engine: audit, research, rebuild, fact-check, check it is different, compare" width="100%"></p>
<p align="center"><img src="assets/sys-ledger.svg" alt="Ledger: import events, tag every number, separate agent work, measured or derived, dashboard" width="100%"></p>

## IDX: the cockpit for the fleet

A Mac cockpit for people who run **Claude Code** and **Gemini CLI** across many projects. Every session is a chat first, the terminal is one click away, and sessions survive a restart. It runs over your own CLIs and accounts. Closed beta.

<p align="center">
<a href="https://emberyard.github.io/idx-site/">
<picture>
<source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emberyard/idx-site/main/public/img/hero-dark-1280.webp">
<img src="https://raw.githubusercontent.com/emberyard/idx-site/main/public/img/hero-light-1280.webp" alt="IDX: a chat-first cockpit for Claude Code and Gemini CLI sessions" width="100%">
</picture>
</a>
</p>
<p align="center"><sub>Screenshot from the IDX site. Demo data only.</sub></p>

<p align="center"><img src="assets/arch.svg" alt="IDX architecture: renderer, desktop shell, host daemon, adapters for Claude Agent SDK, Gemini over ACP and a terminal" width="100%"></p>

## Proof I test my own work

<p align="center"><img src="assets/impact.svg" alt="97 to 86 percent, 57 percent, 9 to 4.5, 80 percent" width="100%"></p>

<details>
<summary><b>Research notebook: three studies and the smaller findings</b></summary>

### A small test flattered the judge

<p align="center"><img src="assets/judge.svg" alt="Bar chart: 97 percent on a 34-site test, about 86 and 85 percent on fresh sites, about 91 percent for a two-stage cascade" width="100%"></p>

My first bake-off of vision models said 97%. On fresh sites the same judge was about 86%. So the rule became: validate on fresh data before any big run, and use a cheap judge first with a stronger one only where it is unsure. My own earlier labels were part of the problem: 5 of 15 sites I had marked "dated" looked modern, so I demoted them from truth to a weak prior.

### Prompting a small image model: the intuitive moves failed

<p align="center"><img src="assets/prompts.svg" alt="Eleven narrow questions scored 0.40 to 0.68; one holistic question scored 0.94" width="100%"></p>

A longer checklist made the model worse. One holistic question beat eleven specific ones, and the order of the answer options alone moved accuracy by seven points.

### AI-built redesigns all look alike

<p align="center"><img src="assets/sameness.svg" alt="57 percent of previews had a same-template look-alike; top font share fell from 49 to 22 percent after a fix" width="100%"></p>

String-level uniqueness is not diversity. Over half of the previews had a look-alike, and one display serif headed 44% of them. That became a quality bar before scale.

### Smaller findings

| Finding | What it changed |
|---|---|
| **Invented claims.** Only 9% of first-wave AI rebuilds passed a fact-check, with a median of 9 to 10 invented claims each. A better brief and filtered inputs brought the median to 4.5. | Truthfulness, not looks, became the quality gate. |
| **Where agent spend goes.** About 80% was subagents, and 97% of tokens were cache reads, so long context re-read on every request drives cost. A naive log parser undercounts output by 2 to 3 times. | Cheaper default model for agents, leaner briefs, shorter sessions. |
| **Tool-reported email opens measure scanners, not people.** Privacy proxies and security scanners "open" mail within seconds. | Never call a lead hot on opens alone. |
| **A delivery test went green while every email body was empty.** I only caught it by reading what the recipient received. | Tests assert the received content, not just placement. |
| **Batching did not speed up a mixture-of-experts model on a Mac.** Each request routes to different experts, so every step reads most of the model. | Paused that plan and moved model tests to cloud GPUs. |
| **Rules did not detect dated sites.** Missing viewport tags and old copyright years were rare; the site builder used was no signal. | The judge has to be visual. |

</details>

## What I am working on

<p align="center"><img src="assets/board.svg" alt="Doing now, next, parked on purpose" width="100%"></p>

## Where the work has been

<p align="center"><img src="assets/timeline.svg" alt="Career timeline 2017 to 2026" width="100%"></p>

<p align="center"><img src="assets/stack.svg" alt="TypeScript, JavaScript, Python, SQL, Node.js, React, Electron, Next.js, Astro, SQLite, JSON-RPC, zod, WebSocket, Claude Agent SDK, Gemini ACP, MCP, PTY" width="100%"></p>

<sub>[M] = measured from a result file I kept. [N] = from my own research notes; the raw files were not re-opened for this page. Small samples, one reviewer: read the percentages as indicative. Private repos are described, not shown. IDX is a working name.</sub>
