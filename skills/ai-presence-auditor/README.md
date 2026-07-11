# AI Presence Auditor

Check whether your local or home-service business shows up when customers ask AI assistants
(ChatGPT, Perplexity, Google AI Overviews, Gemini, Copilot) to recommend a provider — and get the
specific fixes that move the needle. Answer-Engine / Generative-Engine Optimization (**AEO / GEO**)
for local, packaged as an agent skill.

## Why it matters

People increasingly ask AI *"who should I call for a plumber in Austin?"* instead of scrolling Google.
AI names only a handful of businesses — **you're either in the answer or you're invisible.** And there
is no single place to optimize: ChatGPT leans on **Bing + your website + Yelp/Foursquare**, while
Google's AI (AI Overviews, Gemini) leans on your **Google Business Profile**. This skill audits where
you stand across all of those surfaces and hands back a prioritized fix list.

## How AI picks local businesses

| Assistant | Reads mostly from |
| --- | --- |
| ChatGPT | the Bing index + your website + Yelp / Foursquare data (not primarily Google Business Profile) |
| Google AI Overviews / AI Mode / Gemini | your Google Business Profile + the local pack |
| Microsoft Copilot | the Bing ecosystem |
| Siri / Apple Maps | Apple Business Connect |

Ground rules the fixes follow from:

- AI recommends a **small set (~3–5)** of businesses, and often **not** the Google #1 — being *cited*
  is not the same as being *recommended*.
- **Reviews act as a trust filter** (roughly 4+ stars is table stakes); thin or below-average profiles
  get left out.
- **Consistent name/address/phone** across Google, Bing, Apple, Foursquare, and Yelp matters more than
  any single listing.
- **Honest reality check:** AI-sourced recommendations are still a small share of local demand today
  versus the Google local pack and the phone. A growing edge, not the whole game.

## Install

Via [skills.sh](https://skills.sh/OptimizerTeam/agent-skills):

```bash
npx skills add OptimizerTeam/agent-skills
```

Or manually (agent skills live in `~/.claude/skills/` or a project's `.claude/skills/`):

```bash
git clone https://github.com/OptimizerTeam/agent-skills
cp -r agent-skills/skills/ai-presence-auditor ~/.claude/skills/
```

Then ask your agent to **"run the ai-presence-auditor skill for {business} in {city}."**

## Usage

Give it your business name, primary service, city / service area, website, and 2–3 competitors. It
runs representative buyer prompts across AI assistants, diagnoses the surfaces AI pulls from, and
returns a prioritized fix list ranked by impact × effort — plus which competitor AI names instead of
you, and the most likely reason.

## Built by Optimizer

[Optimizer](https://optimizer.team) (optimizer.team) is the AI agent that helps local and home-service
businesses get found — across Google, their website, AI search, and reviews. This skill is the manual,
do-it-yourself version; Optimizer automates the audit, the fixes, and the weekly loop, with the owner
approving every change.

## License

[MIT](../../LICENSE) © Optimizer Team, Inc.
