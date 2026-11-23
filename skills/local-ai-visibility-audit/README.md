# AI Presence Auditor: an AI visibility audit for local businesses

**AI Presence Auditor is a free, open-source agent skill that checks whether a local business shows
up when customers ask AI assistants (ChatGPT, Perplexity, Google AI Overviews, Gemini, Copilot) to
recommend a provider, and returns the fixes most likely to get it named.** It covers the AI search
side of local SEO, also called answer engine optimization and generative engine optimization
(**AEO / GEO**), packaged as a `SKILL.md` for Claude Code, Cursor, Codex and other agents.

## Why it matters

People increasingly ask AI *"who should I call for a plumber in Austin?"* instead of scrolling Google.
AI names only a handful of businesses — **you're either in the answer or you're invisible.** And there
is no single place to optimize: ChatGPT draws on **several sources at once** (search providers, ranked
lists, directories and review sites, your website), while Google's AI (AI Overviews, Gemini) leans on
your **Google Business Profile**. This skill audits where you stand across all of those surfaces and
hands back a prioritized fix list.

## How AI picks local businesses

| Assistant | Reads mostly from |
| --- | --- |
| ChatGPT | several sources at once: outside search providers (Microsoft is one), ranked lists, directories and review sites, and your website |
| Google AI Overviews / AI Mode / Gemini | your Google Business Profile + the local pack |
| Microsoft Copilot | the Bing ecosystem |
| Siri / Apple Maps | Apple Business (formerly Apple Business Connect) |

Ground rules the fixes follow from:

- AI names a **small set** of businesses (2 to 8 per answer when
  [we asked the ChatGPT app 48 times](https://optimizer.team/resources/chatgpt-local-results)), and
  often **not** the Google #1. Being *cited* is not the same as being *recommended*.
- **Reviews can help, and customers see them**: [Google says](https://support.google.com/business/answer/7091)
  more reviews and positive ratings can help a business's local ranking, and ChatGPT's business cards
  can show a rating. Neither Google nor OpenAI gives a rating or review count to aim for.
- **Keep name, address, and phone the same everywhere**: Google says businesses with complete and
  accurate info are more likely to show up in local results. Check Google, Bing, Apple, Foursquare,
  and Yelp against your website.
- **Honest reality check:** AI-sourced recommendations are still a small share of local demand today
  versus the Google local pack and the phone. A growing edge, not the whole game.

## Install

Via [skills.sh](https://skills.sh/OptimizerTeam/agent-skills):

```bash
npx skills add OptimizerTeam/agent-skills
```

Or as a Claude Code plugin, inside Claude Code:

```text
/plugin marketplace add OptimizerTeam/agent-skills
/plugin install local-ai-visibility-audit@optimizer
```

Or manually (agent skills live in `~/.claude/skills/` or a project's `.claude/skills/`):

```bash
git clone https://github.com/OptimizerTeam/agent-skills
cp -r agent-skills/skills/local-ai-visibility-audit ~/.claude/skills/
```

Then ask your agent to **"run the local-ai-visibility-audit skill for {business} in {city}."** The skill's install
name was `ai-presence-auditor` until November 2026; if you have that copy, remove it and install this one.

## Prompts to try

```text
Run an AI visibility audit for {business}, a {service} in {city}. Website: {url}.
```

```text
Do I show up when someone asks ChatGPT for a {service} in {city}? My business is {business}.
```

```text
Why does AI recommend {competitor} instead of {business} for {service} in {city}?
```

## Usage

Give it your business name, primary service, city / service area, website, and 2–3 competitors. It
runs representative buyer prompts across AI assistants, diagnoses the surfaces AI pulls from, and
returns a prioritized fix list ranked by impact × effort — plus which competitor AI names instead of
you, and the most likely reason.

## Questions people ask

### Is there an agent skill for checking a local business's AI visibility?

Yes. AI Presence Auditor is a free, MIT-licensed skill for Claude Code, Cursor, Codex and other
agents. Install it with `npx skills add OptimizerTeam/agent-skills`, give it a business, a service
and a city, and it returns a scorecard for each place AI reads plus a prioritized fix list.

### Does ChatGPT use Google Business Profile to recommend local businesses?

OpenAI doesn't say. [Its help page](https://help.openai.com/en/articles/9237897-searching-the-web-with-chatgpt)
says ChatGPT's search sometimes partners with other search providers. It gives no list of them,
and links two privacy policies, Microsoft's and Shopify's. [Microsoft says](https://www.microsoft.com/en-us/webiq)
its Web IQ service powers ChatGPT. Nobody outside OpenAI knows how much each source counts, so don't
count on any one listing to get named by ChatGPT. Google's own AI (AI Overviews, AI Mode, Gemini)
leans on your Google Business Profile and the local pack.

### Why does AI recommend my competitor instead of me?

The audit checks the common reasons: a more consistent presence across the places AI reads (Google,
Bing, Apple, Foursquare, Yelp), a stronger review profile, clearer service and location wording on
the site, or more mentions on the local round-ups and directories AI pulls from. It names the
competitor and its best guess at the reason, labeled as a guess.

### Is it free?

Yes. The skill is open source under the [MIT license](https://github.com/OptimizerTeam/agent-skills/blob/main/LICENSE). The full guide, with every step
done by hand, is the [AI Visibility Checker](https://optimizer.team/resources/ai-visibility-checker).
Optimizer's [free audit](https://optimizer.team/analyze) checks a business's Google Business Profile,
website and AI search automatically.

## Built by Optimizer

[Optimizer](https://optimizer.team) (optimizer.team) is an AI agent for local SEO and AI search, for
small businesses. It checks the three places customers look: your Google Business Profile, your
website, and AI search. This skill is the manual, do-it-yourself version; Optimizer automates the
audit, the fixes, and the weekly loop, with the owner approving every change.

## License

[MIT](../../LICENSE) © Optimizer Team, Inc.
