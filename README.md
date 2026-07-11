# AI Presence Auditor — a Claude skill

Check whether your local or home-service business shows up when customers ask AI assistants
(ChatGPT, Perplexity, Google AI Overviews, Gemini, Copilot) to recommend a provider — and get the
specific fixes that move the needle. This is Answer-Engine / Generative-Engine Optimization
(**AEO / GEO**) for local businesses, packaged as a Claude skill.

## Why it matters

People increasingly ask AI *"who should I call for a plumber in Austin?"* instead of scrolling Google.
AI names only a handful of businesses — **you're either in the answer or you're invisible.** And there
is no single place to optimize: ChatGPT leans on **Bing + your website + Yelp/Foursquare**, while
Google's AI (AI Overviews, Gemini) leans on your **Google Business Profile**. This skill audits where
you stand across all of those surfaces and hands back a prioritized fix list.

## How AI picks local businesses (what the audit is based on)

There is no single "AI" — different assistants read different sources, so getting found by AI is a
multi-surface job:

| Assistant | Reads mostly from |
| --- | --- |
| **ChatGPT** | the Bing index + your website + Yelp / Foursquare data (not primarily Google Business Profile) |
| **Google AI Overviews / AI Mode / Gemini** | your Google Business Profile + the local pack |
| **Microsoft Copilot** | the Bing ecosystem |
| **Siri / Apple Maps** | Apple Business Connect |

Ground rules the fixes follow from:

- AI recommends a **small set (~3–5)** of businesses, and often **not** the Google #1 — being *cited*
  is not the same as being *recommended*.
- **Reviews act as a trust filter** (roughly 4+ stars is table stakes); thin or below-average profiles
  get left out.
- **Consistency across sources** (matching name/address/phone on Google, Bing, Apple, Foursquare, Yelp)
  matters more than any single listing.
- **Honest reality check:** AI-sourced recommendations are still a small share of local demand today
  versus the Google local pack and the phone. This is a growing edge, not the whole game.

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
returns a prioritized fix list ranked by impact × effort — plus which competitor AI names instead of
you, and the most likely reason.

## FAQ

### Does ChatGPT use Google Business Profile to recommend local businesses?
Mostly no. ChatGPT's local answers lean on the **Bing** search index plus your website and Yelp /
Foursquare data. Your **Google Business Profile** drives Google's own AI (AI Overviews, Gemini) and the
local pack — not ChatGPT. Getting found by AI means covering both.

### Why does AI recommend my competitor instead of me?
Usually because the competitor has more **consistent presence across the sources AI reads** (Google,
Bing, Apple, Foursquare, Yelp), a stronger **review** profile, clearer **service + location** copy, or
more **third-party citations** ("best-of" lists, directories). The audit shows which competitor is named
and the most likely reason.

### How do I get my business recommended by ChatGPT or found by AI?
Claim and complete your listings across **Google Business Profile, Bing Places, Apple Business Connect,
Foursquare, and Yelp**; keep your name/address/phone consistent; keep reviews recent and above average;
say exactly **what you do and where** in plain text on your site; and earn mentions on the local sites
AI pulls from. This skill audits all of that.

### Does my Google ranking still matter for AI search?
Indirectly. AI names only a handful of businesses and often not the Google #1, so a top Google ranking
does not guarantee you're the name the AI says out loud. Google visibility helps the Google AI surfaces
(AI Overviews, Gemini); ChatGPT depends more on Bing, your website, and third-party data.

### How many businesses does AI recommend?
Typically a **small handful (~3–5)** per query — "winner-take-few." Unlike a Google results page where
you can be #7 and still get clicks, in an AI answer you're either named or you don't exist.

### Do reviews affect AI recommendations?
Yes. AI treats reviews as a **trust filter** — roughly 4+ stars, with recent and answered reviews, is
table stakes. There's no proven exact numeric cutoff, so don't chase a magic number; keep a steady
review habit.

### What are AEO and GEO?
**Answer Engine Optimization (AEO)** and **Generative Engine Optimization (GEO)** are the practice of
getting your business surfaced and cited in AI-generated answers (ChatGPT, Perplexity, Google AI),
rather than only ranking in traditional search results.

### Is this free?
Yes — the skill is open source under the [MIT license](./LICENSE).

## Built by Optimizer

[Optimizer](https://optimizer.team) is the AI agent that helps local and home-service businesses get
found — across Google, their website, AI search, and reviews. This skill is the manual, do-it-yourself
version; Optimizer automates the audit, the fixes, and the weekly loop, with the owner approving every
change.

## License

[MIT](./LICENSE) © Optimizer Team, Inc.
