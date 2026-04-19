---
title: "Your Website Has One of Two AI Visibility Problems"
description: "After auditing seven companies for AI search readiness, a clear pattern emerged: every site falls into one of two categories — schema-gap or content-gap. The diagnosis determines whether the fix takes a week or six months."
pubDate: 'Apr 19 2026'
tags: ['geo', 'structured-data', 'content-strategy', 'ai-search', 'diagnostics']
---

After seven GEO audits — across fintech, HR tech, legal tech, e-commerce, and SaaS — I expected to find seven different problems. Instead I found two.

Every company with weak AI visibility has one of two root causes, and they require completely different fixes. Confusing one for the other wastes months. Getting the diagnosis right means you can fix the actual problem in a fraction of the time.

## The Two Types

**Schema-gap companies** have great content but terrible machine-readability. They've invested in blog posts, comparison pages, FAQ sections, case studies, glossaries. A human reading their site would understand exactly what the company does, who it's for, and how it compares to alternatives. An AI model parsing their structured data finds almost nothing.

**Content-gap companies** have the opposite problem — or more accurately, they have both problems at once. They haven't created the content that AI models need to form opinions, AND they don't have structured data wrapping what little content exists. The machine-readability problem is real, but it's secondary. You can't mark up content that doesn't exist.

This distinction matters because the fix for a schema-gap company is surgical and fast. The fix for a content-gap company is strategic and slow. And the worst thing you can do is apply the wrong fix.

## What Schema-Gap Looks Like in Practice

FreshBooks scored 62/100 on our GEO audit. Their content was excellent — detailed comparison pages against QuickBooks and Xero, FAQ sections covering pricing and features, a blog with hundreds of educational articles. A marketing team had clearly invested years in building this content library.

Their structured data score? 55/100.

All that comparison content lived as plain HTML. No FAQPage schema on their FAQ sections. No SoftwareApplication schema on their product pages. No structured comparison markup on their "FreshBooks vs QuickBooks" page. The content was doing the right work for human visitors and doing almost nothing for AI extraction.

Wealthsimple had a similar pattern at a higher level. They scored 75/100 overall, with rich Organization and FinancialService schema on their homepage — but their investment product pages, which contain exactly the kind of structured information AI models love (fee schedules, account types, eligibility requirements), had minimal markup beyond the basics.

Clio, the legal practice management platform, followed the same pattern. Strong content library, solid authority in the legal tech space, but WordPress-generated schema doing the minimum rather than capturing the depth of information already on the page.

The common thread: these companies had already done the hard part. They'd invested in content. The AI visibility problem was a technical implementation gap, not a content strategy gap.

## What Content-Gap Looks Like in Practice

Allbirds scored 58/100. Not because their structured data was notably worse than FreshBooks' — it was only slightly worse. The real gap was content.

When someone asks an AI "what are the most sustainable running shoes?" the model needs source material to form a recommendation. It needs comparison content, detailed product specifications, sustainability methodology explanations, FAQ content addressing common questions. Allbirds had a brand story. They didn't have the structured, queryable content library that AI models use to build confident answers.

Their homepage was a visual experience — beautiful imagery, minimal text, brand-forward design. For human visitors in a discovery mindset, it works. For an AI crawler trying to extract facts about material sourcing, carbon footprint data, product specifications, and competitive positioning, it's a desert.

Roam, a car subscription service, scored 48/100 — our lowest. The site was essentially a conversion funnel: hero section, "how it works," pricing, signup. Almost no educational content. No FAQ sections. No comparison pages. No blog posts explaining the car subscription model vs. leasing vs. buying. The site assumed visitors already understood the category and were ready to convert.

An AI model asked "is a car subscription worth it?" had almost nothing to work with from Roam's site. The answer would be constructed entirely from third-party sources — sources that might or might not present car subscriptions favorably, and that certainly wouldn't present Roam specifically.

## Why the Diagnosis Matters

Here's where companies waste time and money: a content-gap company hires a developer to add schema markup, and a schema-gap company hires a content strategist to write new pages.

### The wrong fix for schema-gap companies

A schema-gap company that commissions a new blog series, a fresh round of comparison pages, or a content overhaul is solving a problem they don't have. Their content is already good. More content won't change AI visibility if the existing content isn't machine-readable.

I've seen this happen. A company audits their AI visibility, sees they're underperforming, and defaults to the familiar playbook: "We need more content." They don't need more content. They need to make their existing content parseable by machines.

### The wrong fix for content-gap companies

Conversely, a content-gap company that adds SoftwareApplication schema to their homepage and FAQPage schema to their (nonexistent) FAQ section has solved nothing. You can't mark up content that isn't there. Schema is a wrapper, not a substitute.

A content-gap company that jumps straight to structured data implementation is putting a frame on an empty canvas. The frame is technically perfect. There's nothing inside it.

### The right sequence

**For schema-gap companies:** Audit existing content → identify high-value pages missing structured data → implement schema markup → validate with testing tools → measure AI mention changes. Timeline: 1-4 weeks depending on site size. This is a developer task with occasional content review.

**For content-gap companies:** Identify the queries AI models are answering about your category → audit what content exists to address those queries → build the missing content (comparison pages, FAQs, educational resources, product specifications) → THEN add structured data markup → measure results. Timeline: 2-6 months. This is a content strategy project with a technical implementation phase at the end.

The schema-gap fix is a sprint. The content-gap fix is a program.

## How to Diagnose Yourself in 15 Minutes

You don't need a full GEO audit to figure out which camp you're in. Here's a quick diagnostic:

**Step 1: Ask an AI about your category.** Go to ChatGPT or Perplexity and ask "What is the best [your category] for [your target customer]?" Read the response carefully.

- If the AI mentions your competitors in detail but not you → content gap. The model doesn't have enough material from your site to form an opinion.
- If the AI mentions you but gets facts wrong or is vague → probably schema gap. The content exists but isn't structured well enough for accurate extraction.
- If the AI mentions you accurately → you might be fine. Or you might be one model update away from losing that mention.

**Step 2: Check your structured data.** Go to Google's Rich Results Test (search.google.com/test/rich-results) and plug in your homepage, your main product page, and your most important FAQ or comparison page.

- If you see only basic Organization/WebSite schema → schema gap (if content is strong) or both gaps (if content is weak).
- If you see rich schema (FAQPage, SoftwareApplication, Product with detailed properties) → your structured data is probably not the bottleneck. Look at content.

**Step 3: Count your "AI-queryable" pages.** How many pages on your site directly answer questions someone might ask an AI? Not brand pages. Not feature tours. Pages with specific, factual, question-and-answer style content.

- More than 20? You probably have a schema gap.
- Fewer than 5? You have a content gap.
- Somewhere in between? Look at which pages rank well in traditional search — those are likely your strongest AI-visible content, and they're probably missing structured data.

## The Spectrum, Not the Binary

In practice, no company is purely one type. Wealthsimple was primarily a schema-gap company but had content gaps on specific product pages. Allbirds was primarily a content-gap company but also had schema gaps on the content that did exist.

The useful framing isn't "which type am I?" but "where should I spend my first month?"

If your content score is strong and your schema score is weak, spend month one on structured data implementation. You'll see results fast because the content foundation is already there.

If both scores are weak, spend months one through three on content — and don't touch schema until you have something worth marking up. Adding structured data to thin content doesn't help. It just makes thin content more precisely thin.

## What the Regulated Industries Teach Us

The most interesting finding across all seven audits: regulated industries consistently showed up as schema-gap companies rather than content-gap companies. Wealthsimple, Clio, and Deel (HR tech, scored 82/100) all had strong content foundations. Regulatory requirements forced them to be precise and thorough in describing their products, pricing, and terms. That precision is exactly what AI models need.

Their gap was always technical, not strategic. They'd created the content because regulators demanded it. They just hadn't wrapped it in structured data because nobody demanded that.

E-commerce and early-stage SaaS, on the other hand, tended toward content-gap. Allbirds' brand-forward minimalism and Roam's conversion-focused design both optimized for human emotional response at the expense of machine-readable substance. Neither industry has a regulatory forcing function toward precision.

The implication: if you're in fintech, legal tech, or healthcare, your AI visibility fix is probably faster and cheaper than you think. The hard work is done. You need a developer for a few weeks, not a content strategist for a quarter.

If you're in e-commerce, D2C, or early-stage SaaS, you probably need the content strategist. And you need them before you need the developer.

## The Cost Difference Is Enormous

A schema-gap fix for a mid-size SaaS company — adding FAQPage schema to existing FAQ sections, SoftwareApplication schema to product pages, structured comparison data to vs-pages — might be 40-80 hours of developer work. At agency rates, call it $8,000-$16,000. At an in-house developer's time allocation, it's a two-week sprint.

A content-gap fix for the same company — building a comparison page library, writing detailed FAQ content, creating educational resources, establishing a glossary, and THEN adding structured data — is a 3-6 month content program. Even with AI-assisted writing, you're looking at strategy, research, writing, review, publishing, and then the technical implementation on top. Easily $30,000-$100,000 in content production costs, or a quarter of a content team's time.

That's a 5-10x difference in cost and a 4-8x difference in timeline. Getting the diagnosis right isn't academic — it's the difference between a line item and a strategic initiative.

## The Diagnostic Question Nobody's Asking

Most companies asking about AI visibility are asking "How do we show up in AI search?" That's the wrong first question.

The right first question is: "Do we have a content problem or a schema problem?"

Everything downstream — budget, timeline, team allocation, expected results, executive buy-in requirements — depends on the answer. A schema-gap company can pitch their leadership on a two-week technical project with fast, measurable results. A content-gap company needs to pitch a multi-month content investment with longer payback periods.

The seven audits taught me that companies fall into these two buckets with surprising consistency. And the companies that get the diagnosis right move faster, spend less, and see results sooner than the ones that default to "we need better AI visibility" without understanding what's actually in the way.

Figure out which problem you have. Then fix that one.
