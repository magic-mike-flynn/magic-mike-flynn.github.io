---
title: 'I Audited 5 Websites for AI Visibility. Here''s What AI Actually Sees.'
description: 'After running GEO audits on a car subscription, a scheduling tool, a shoe company, a law firm platform, and a fintech — concrete patterns emerged about what makes a website visible to AI.'
pubDate: 'Apr 02 2026'
tags: ['geo', 'research', 'building-in-public', 'AI-visibility']
---

Over the past week I've run GEO (Generative Engine Optimization) audits on five companies across five different verticals. Not hypothetical analysis — actual site crawls, schema inspection, AI query testing, the works.

The companies: **Roam** (car subscriptions), **Cal.com** (scheduling SaaS), **Allbirds** (sustainable footwear), **Clio** (legal practice management), and **Wealthsimple** (fintech).

Their GEO scores ranged from 48 to 75 out of 100. Here's what I found.

## The Biggest Gap Is the Same Everywhere: Nobody Talks to AI Crawlers

Zero out of five had an `llms.txt` file. Zero.

For context: `llms.txt` is an emerging standard — a plain text file at your site root that tells AI systems what your company does, what your products are, and what makes you different. Think of it as `robots.txt` for meaning instead of access. It takes maybe 30 minutes to create.

Every single company I audited would benefit from one. Yet none had it. This isn't a technical challenge — it's an awareness gap. Most companies don't realize AI crawlers are visiting their site and trying to understand it, and that there's a simple way to help.

## Regulated Industries Have Better Structured Data (By Accident)

This was the most interesting pattern. Wealthsimple (fintech) had `Organization` + `FinancialService` dual-typing with a 6-product `OfferCatalog` including fee specifications. Clio (legal tech) had moderate WordPress-generated schema with product and pricing markup. Meanwhile, Allbirds (e-commerce on Shopify) had minimal schema, and Cal.com (SaaS) had basic `Organization` only.

The reason is obvious in hindsight: regulated industries are required to be precise about what they offer, what it costs, and what the terms are. That precision naturally translates into richer structured data. Fintech companies list fee structures because regulators make them. Legal tech companies describe their products in detail because lawyers demand it. That structured information is exactly what AI models consume best.

The implication: if you're in e-commerce or early-stage SaaS, you're probably starting from a lower baseline than you think. Your competitors in regulated verticals already have richer schema — not because they're optimizing for AI, but because their industry forces clarity.

## JavaScript Rendering Is an Invisible Killer

Roam scored 48/100 — the lowest of the five — and the biggest reason wasn't content quality or missing schema. It was JavaScript rendering.

Their site uses Webflow with heavy client-side rendering. When I tested what AI crawlers actually see (versus what a browser renders), large chunks of content were invisible. Product listings, pricing information, feature descriptions — all loaded dynamically, all invisible to bots that don't execute JavaScript.

This is a problem that's hard to diagnose because the site *looks* fine to humans. You visit it, everything loads, it looks professional. But AI crawlers and search engines see a skeleton. The content exists but it's behind a JavaScript wall.

Cal.com, by contrast, uses Next.js with server-side rendering — most content is visible to crawlers out of the box. Same modern framework vibes, completely different AI visibility.

If your site is built on Webflow, Wix, or a heavily JS-dependent stack, check what your site looks like with JavaScript disabled. That's closer to what AI sees.

## FAQ Content Without FAQ Schema Is a Missed Layup

Four out of five companies had extensive FAQ-style content — help pages, how-to guides, explainer articles. Clio has an entire legal research library. Wealthsimple has detailed guides on TFSAs, RRSPs, and every financial product they offer. Allbirds has sustainability explainers.

Almost none of it had `FAQPage` schema markup.

This matters because AI systems weigh structured FAQ data heavily when answering user questions. A page titled "What is a TFSA?" with FAQ schema is much more likely to be cited in an AI answer than the same page without it. The content is doing the hard work already — the schema just tells AI systems "this is a direct question-and-answer pair, you can use this."

Adding FAQ schema to existing content is one of the highest-ROI changes a company can make for AI visibility. The content already exists. You're just wrapping it in a format AI can parse cleanly.

## The Comparison Page Gap

When I tested AI queries like "best scheduling software" or "Allbirds vs Nike," the companies with dedicated comparison pages showed up more consistently in AI responses. Cal.com had some comparison content ("Cal.com vs Calendly"). Most others had none.

This is a content strategy gap, not a technical one. People ask AI tools comparative questions constantly: "What's better, X or Y?" "Best [category] for [use case]?" If you don't have a page that directly addresses those queries, AI models will answer using whatever third-party comparison sites or review aggregators they can find. You lose control of your own narrative.

## Score Distribution Tells a Story

| Company | Vertical | Score | Rating |
|---------|----------|-------|--------|
| Roam | Car subscriptions | 48 | 🔴 Needs Work |
| Allbirds | E-commerce | 58 | 🟠 Fair |
| Clio | Legal SaaS | 72 | 🟡 Good |
| Wealthsimple | Fintech | 75 | 🟡 Good |
| Cal.com | Open-source SaaS | 68 | 🟡 Good |

The regulated industries (Clio, Wealthsimple) cluster at the top. E-commerce (Allbirds) sits in the middle. The Webflow-based site (Roam) sits at the bottom despite having a solid product and good content.

This isn't a perfect sample — five companies is a pattern, not a proof. But the consistency is striking. The companies that are forced to be precise and structured by their industry are naturally better positioned for AI visibility. The ones that rely on visual design and dynamic rendering are worse off.

## What This Means

If I had to distill the five audits into one sentence: **AI rewards clarity and structure over design and dynamism.**

A plainly written FAQ page with proper schema will outperform a beautifully designed interactive experience that renders client-side. A detailed product page with explicit pricing and feature lists will beat a slick marketing page with vague value propositions. An `llms.txt` file that takes 30 minutes to write will do more for AI visibility than most SEO consultants' entire recommendations.

The bar for AI optimization is still low. Most companies haven't started. That's the opportunity — and it's the reason I'm building in this space.

---

*These audits are part of building my GEO Snapshot product. If you want to see what AI actually sees when it looks at your website, that's literally what I'm making.*
