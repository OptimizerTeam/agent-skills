# Agent skills for local SEO and AI search

**AI Presence Auditor is a free, open-source (MIT) agent skill that runs an AI visibility audit for a
local business.** It checks whether the business gets named when customers ask ChatGPT, Perplexity,
Gemini, Google's AI Overviews or Copilot who to hire, then returns a prioritized list of fixes. It
works in Claude Code, Cursor, Codex and any other agent that loads `SKILL.md` skills. Published by
**[Optimizer](https://optimizer.team)** (optimizer.team).

[![skills.sh](https://skills.sh/b/OptimizerTeam/agent-skills)](https://skills.sh/OptimizerTeam/agent-skills)

## Install

```bash
npx skills add OptimizerTeam/agent-skills
```

Then ask your agent:

```text
Run an AI visibility audit for {business}, a {service} in {city}. Website: {url}.
```

## Available skills

### [ai-presence-auditor](./skills/ai-presence-auditor)

Checks whether a local or home-service business shows up when customers ask AI assistants (ChatGPT,
Perplexity, Google AI, Gemini, Copilot) to recommend a provider, then returns a prioritized list of
fixes across the places AI reads (Google Business Profile, Bing Places, Apple Business, Foursquare,
Yelp).

**Use when:**

- Auditing whether a business appears in AI answers (AEO / GEO)
- Answering "do I show up in ChatGPT?" or "why does AI recommend my competitor?"
- Finding the highest-impact fixes to get recommended by AI

Skill page: [skills.sh/optimizerteam/agent-skills/ai-presence-auditor](https://skills.sh/optimizerteam/agent-skills/ai-presence-auditor).
Full guide, with every step done by hand: [AI Visibility Checker](https://optimizer.team/resources/ai-visibility-checker).

## About Optimizer

[Optimizer](https://optimizer.team) is an AI agent for local SEO and AI search, for small businesses.
It checks the three places customers look (your Google Business Profile, your website, and AI search)
and hands over evidence-backed fixes that the owner approves before anything changes. A product of
Optimizer Team, Inc.

## License

[MIT](./LICENSE) © Optimizer Team, Inc.
