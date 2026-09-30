---
name: ai-presence-auditor
description: Audit whether a local or home-service business shows up when customers ask AI assistants (ChatGPT, Perplexity, Google AI Overviews/AI Mode, Gemini, Copilot) to recommend a provider — and produce the specific, prioritized fixes that move the needle. Use for an AEO/GEO audit of a local business, or when someone asks "do I show up in ChatGPT," "why does AI recommend my competitor," or "how do I get found by AI."
---

# AI Presence Auditor

Customers increasingly ask an AI assistant "who should I call for a plumber in Austin?" instead of
scrolling Google. AI names only a **handful** of businesses — you're either in the answer or you're
invisible. This skill audits where a local business stands across the surfaces AI actually reads, and
returns a prioritized list of fixes.

## What you need (inputs)

- Business name
- Primary service(s)
- City / service area
- Website URL
- 2–3 competitors (optional but useful)

## How AI actually picks local businesses (the model the fixes follow from)

There is **no single "AI"** — different assistants read different sources, so "get found by AI" is a
multi-surface job, not one listing:

- **ChatGPT** leans on the **Bing index** + your website + Yelp/Foursquare structured data — *not*
  primarily Google Business Profile.
- **Google AI Overviews / AI Mode / Gemini** lean on your **Google Business Profile** + the local pack.
- **Microsoft Copilot** ← the Bing ecosystem. **Siri / Apple Maps** ← **Apple Business Connect**.

A few ground rules that shape every recommendation:

- AI recommends a **small set (~3–5)** of businesses, and often **not** the Google #1. Being *cited* is
  not the same as being *recommended*.
- **Reviews act as a trust filter** — roughly 4+ stars is table stakes; thin or below-average review
  profiles get left out. (There's no proven exact numeric cutoff — don't invent one.)
- **Multi-source consistency** beats any single listing: consistent name/address/phone (NAP) across
  Google, Bing, Apple, Foursquare, Yelp, and directories is what lets the AI trust the entity.
- **Reality check:** AI-sourced recommendations are still a **small share** of local demand today versus
  the Google local pack and the phone. Treat this as a growing edge, not the whole game — and say so.

## The audit

1. **Run representative buyer prompts.** Across ChatGPT + Perplexity + Google AI (and Gemini/Copilot if
   available), use real customer phrasing: "best emergency plumber in {city}", "who should I call for
   {problem} in {city}", "top-rated {service} near {neighborhood}". For each prompt record: Is the
   business named? Which competitors are named? What reason or source does the AI give?
2. **Diagnose the surfaces.** Check presence + completeness on **Google Business Profile, Bing Places,
   Apple Business Connect, Foursquare, and Yelp.** Flag any that are missing or unclaimed.
3. **Check NAP consistency** (name, address, phone) across those registries — mismatches confuse the
   entity and suppress recommendations.
4. **Check reviews** — volume, recency, average rating, and response rate. Below-average or thin →
   likely filtered out regardless of everything else.
5. **Check the website.** Does it state, in plain text, exactly what you do and where ("24/7 emergency
   plumbing in {city}")? Are there service and service-area pages, and an FAQ that matches how people
   ask AI? Vague "quality solutions for all your needs" copy is effectively invisible to AI.
6. **Check third-party mentions/citations** — is the business named in local "best-of" round-ups,
   directories, and review sites the AI pulls from?

## Output

- A short **scorecard per surface** (present / missing / needs work).
- **"Where you're missing vs where AI actually looks."**
- A **prioritized fix list** ranked by impact × effort — quick wins first (e.g., claim Bing Places, fix
  a NAP mismatch, add a service-area page, start a review-a-week habit).
- **Which competitor the AI names instead**, and the most likely reason.
- An honest framing line: this is a growing edge — don't abandon Google/GBP or the phone.

## Guardrails

- **Evidence-based only.** Never fabricate rankings, review counts, citations, or percentages you did
  not actually verify.
- **Recommend; the owner approves and publishes.** No surprise changes.
- **Keep the numbers honest** — AI's share of local demand is still small; don't overstate urgency.

---

Built by **[Optimizer](https://optimizer.team)** — the AI agent that helps local and home-service
businesses get found across Google, their website, and AI search. This skill is the manual,
do-it-yourself version of the audit; Optimizer automates the checks, the fixes, and the weekly loop —
with the owner approving every change.
