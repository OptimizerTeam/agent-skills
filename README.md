# AI Presence Auditor — a Claude skill

Check whether your local or home-service business shows up when customers ask AI assistants
(ChatGPT, Perplexity, Google AI, Gemini, Copilot) to recommend a provider — and get the specific
fixes that move the needle. Answer-Engine / Generative-Engine Optimization (AEO/GEO) for local.

## Why

People increasingly ask AI *"who should I call for a plumber in Austin?"* instead of scrolling Google.
AI names only a handful of businesses — **you're either in the answer or you're invisible.** And there's
no single place to optimize: ChatGPT leans on **Bing + your website + Yelp/Foursquare**, while Google's
AI (AI Overviews, Gemini) leans on your **Google Business Profile**. This skill audits where you stand
across all of those surfaces and hands back a prioritized fix list.

## Install

Claude skills live in `~/.claude/skills/` (global) or `.claude/skills/` (per-project):

```bash
git clone https://github.com/OptimizerTeam/ai-presence-skill
cp -r ai-presence-skill/skills/ai-presence-auditor ~/.claude/skills/
```

Then, in Claude: **"run the ai-presence-auditor skill for {business} in {city}."**

## Usage

Give it your business name, primary service, city / service area, website, and 2–3 competitors. It
runs representative buyer prompts across AI assistants, diagnoses the surfaces AI pulls from, and
returns a prioritized fix list ranked by impact × effort.

## What it checks

- **Presence + NAP consistency** across Google Business Profile, Bing Places, Apple Business Connect,
  Foursquare, and Yelp
- **Reviews** — volume, recency, and rating (AI treats reviews as a trust filter)
- **On-page clarity** — clear service + location copy, service-area pages, FAQ
- **Third-party citations** — "best-of" round-ups, directories, and review sites AI pulls from

## Built by Optimizer

[Optimizer](https://optimizer.team) is the AI agent that helps local and home-service businesses get
found — across Google, your website, AI search, and reviews. This skill is the manual version;
Optimizer automates the audit, the fixes, and the weekly loop, with the owner approving every change.

## License

[MIT](./LICENSE) © Optimizer Team, Inc.
