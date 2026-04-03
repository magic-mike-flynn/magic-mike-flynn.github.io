---
title: 'AI Is Answering Competitive Questions About Your Product. Are You?'
description: 'When someone asks ChatGPT "FreshBooks vs QuickBooks," who controls the answer? After 6 GEO audits, I found that comparison content is the most underrated AI visibility strategy — and most companies are ceding their narrative to third parties.'
pubDate: 'Apr 03 2026'
tags: ['geo', 'research', 'AI-visibility', 'content-strategy']
---

Here's what happens when someone asks ChatGPT "FreshBooks vs QuickBooks":

The model looks for the most structured, authoritative comparison it can find. If FreshBooks has a dedicated page at `/compare/quickbooks-vs-freshbooks` with clear feature comparisons, pricing breakdowns, and honest positioning — that page has a strong chance of shaping the answer. If they don't, ChatGPT pulls from G2 reviews, Reddit threads, random blog posts, and whatever comparison sites rank well.

One of those scenarios gives you control of your narrative. The other gives it to strangers.

## The Pattern Across 6 Audits

I've now run GEO audits on six companies: Roam, Cal.com, Allbirds, Clio, Wealthsimple, and FreshBooks. Across five verticals, different sizes, different tech stacks. And the single most consistent predictor of whether a company shows up well in competitive AI queries isn't their domain authority or their schema markup — it's whether they have dedicated comparison content.

**FreshBooks** has five dedicated comparison pages in their main navigation: vs QuickBooks, vs Xero, vs Wave, vs HoneyBook, vs Harvest. Plus 13 industry-specific landing pages for freelancers, construction, legal, creatives, and more. They scored 62/100 overall, but their content architecture sub-score was 17/20 — the highest in my portfolio.

**Cal.com** has some "Cal.com vs Calendly" content. Not as comprehensive, but it exists. When you ask AI systems about scheduling tool alternatives, Cal.com shows up.

**Allbirds** has nothing. No "Allbirds vs Nike" page. No "best sustainable sneakers" comparison. When someone asks an AI "should I buy Allbirds or Nike," the answer is built entirely from third-party sources. Allbirds scored 58/100 — and the content gap is a major reason why.

## Why Comparison Queries Matter More Than You Think

People don't ask AI for homepages. They ask it questions. And the most commercially valuable questions are comparative:

- "Best accounting software for freelancers"
- "Allbirds vs Nike sustainability"
- "Calendly vs Cal.com for teams"
- "Is Wealthsimple good for beginners?"

These are buying-intent queries. The person asking has already narrowed their options and is looking for a tiebreaker. If your company is part of the answer — and the answer reflects your positioning — you're in the game. If you're absent, you're invisible at the exact moment someone is deciding.

Traditional SEO taught companies to optimize for category keywords. GEO demands you optimize for *questions* — specifically, the questions people are already asking AI about you and your competitors.

## The Honest Comparison Advantage

There's a counterintuitive element here. The best comparison pages aren't the ones that claim victory on every dimension. They're the ones that are honest.

FreshBooks' comparison pages acknowledge where competitors are strong. Their "vs QuickBooks" page doesn't pretend QuickBooks doesn't exist or isn't powerful. It positions FreshBooks as better for small businesses and freelancers while acknowledging QuickBooks' strength for larger operations.

AI models are trained on enormous corpora. They can cross-reference claims. A comparison page that says "we're better at everything" gets weighted against the mountain of evidence suggesting otherwise. A page that says "we're better at X and Y, they're better at Z, here's how to decide" reads as authoritative and balanced. AI systems are more likely to cite it because it aligns with what the models already know from other sources.

Honesty isn't just ethical in comparison content. It's strategically optimal for AI visibility.

## The Schema Layer Most Companies Skip

Here's where it gets technical — and where the opportunity gets bigger.

FreshBooks has excellent comparison content. But none of it has `ItemList` or `Table` schema markup. The comparisons exist as prose and HTML tables that humans can read, but AI crawlers have to parse and interpret.

This matters because structured data is how you make comparisons *machine-parsable*. An `ItemList` with explicit feature comparisons tells an AI system exactly what's being compared and on what dimensions. Without it, the AI has to extract that information from unstructured text — which it can do, but less reliably, and with less confidence.

The same pattern shows up with FAQ content. Four of the six companies I've audited have extensive FAQ sections. Almost none have `FAQPage` schema. The questions and answers exist — they're just not wrapped in a format that AI systems can parse cleanly.

If you already have comparison pages and FAQ content, adding the structured data layer is one of the highest-ROI things you can do for AI visibility. The hard work (creating the content) is done. The easy work (marking it up) is what's missing.

## What This Means Practically

If I'm a marketing leader reading this, here's what I'd do Monday morning:

**1. Search for yourself in AI.** Open ChatGPT, Claude, or Perplexity and type "[your company] vs [main competitor]." Then try "[your category] for [your target customer]." What comes back? Is it accurate? Is it yours?

**2. Create comparison pages.** For your top 3-5 competitors, create dedicated pages: `/compare/you-vs-competitor`. Be specific. Include features, pricing, ideal customer profiles. Be honest about where the competitor is strong.

**3. Create use-case pages.** If your product serves multiple verticals or personas, create landing pages for each: `/for-freelancers`, `/for-agencies`, `/for-enterprise`. These match how people ask AI for recommendations: "best [tool] for [my situation]."

**4. Add structured data.** If you already have comparison or FAQ content, add `ItemList`, `FAQPage`, and `SoftwareApplication` schema. This is the technical layer that makes your content machine-readable.

**5. Create an llms.txt file.** In 30 minutes, you can create a plain text file at your site root that tells AI crawlers who you are, what you do, and what makes you different. Zero of six companies in my audit portfolio have one.

## The Underlying Shift

Traditional marketing assumed you controlled the narrative because you controlled the channels. Your website, your ads, your PR. GEO flips that assumption. AI systems are synthesizing answers from the entire internet, and the user never visits your website at all.

The companies that win in this environment aren't the ones with the best design or the most ad spend. They're the ones whose information is the most structured, the most honest, and the most directly responsive to the questions people actually ask.

Comparison content is the clearest example of this shift. You either answer the competitive question yourself — in a format AI can understand — or you let the internet answer it for you.

---

*I'm building GEO intelligence tools to help companies see what AI actually sees when it looks at their website. If that sounds useful, [stay tuned](https://magic-mike-flynn.github.io).*
