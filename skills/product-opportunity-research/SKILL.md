---
name: dativue-product-opportunity-research
description: Use Dativue to find underserved customer problems in a niche, compare existing solutions, inspect payment evidence, and recommend a demand test before building a product.
---

# Dativue product opportunity research

Use this for niche-first product discovery and a decision about what to test before building.
Research competing products and services without requiring an app-store choice or app-store retrieval.

## Scope and spending

Reuse the supplied niche, customer, country, language, and decision.
Ask one concise round only for missing essentials; wait for those answers before research.
Quote a bounded plan with `research_credit_quote` before paid calls.
Keep the full run, including retries and follow-ups, within 50 credits or the user's lower limit.
Track settled charges plus outstanding maximum holds against that limit.
Released search holds can fund follow-ups only after their quoted maximum fits the remaining budget.
Narrow the sample when necessary and disclose the resulting coverage limit.

A useful starting plan is one TikTok search and comments from two videos, one Reddit search and comments from up to six threads, up to two exact Reddit post reads, three basic keyword batches, up to three basic SERPs, and one basic public-review request.
Adapt that mix to source relevance and the quoted prices; leave room for discovery corrections.
For pending results, poll the exact `jobId` with `research_job_status`, rather than repeating the paid request.

## Evidence collection

Start with relevant TikTok content and Reddit discussions, then read comments from a small selection of substantive sources.
Use `social_search`, `social_comments`, and `social_get` for exact public posts.
When discovery is noisy, use available web discovery for candidate URLs, then retrieve those exact URLs through Dativue.
If web discovery is unavailable, disclose that limit instead of fabricating sources.

Separate recurring frustrations, attempted workarounds, requested solutions, and spending evidence.
Exclude promotions, moderation bots, generic reactions, and deleted placeholders from substantive buyer evidence.
Do not treat a selected sample as a prevalence estimate or count repeated records from the same source as independent buyers.

Find competing products and services through `search_serp` and public community recommendations.
Inspect available public reviews with `search_reviews`, and verify important feature and price claims on official websites using available web tools.
For Trustpilot, pass the business domain as `target`, rather than the Trustpilot review-page URL.
Label dynamic prices, unavailable review sources, untested vendor claims, and any competitor whose reviews were not retrieved.
Check whether native tools, free resources, services, or existing workflows already solve the problem.

Use `search_keyword_ideas` with no more than five seeds per call.
Preserve country, language, metric dates, estimated monthly volume, and unavailable fields as `N/A`.
Keep measured search activity separate from inferred product demand; do not add overlapping volumes into market size.

## Decision and demand test

Preserve original URLs, publication and collection dates, short excerpts, source-level sample sizes, and retrieval limitations.
Country and language search settings do not establish the location or identity of social commenters or reviewers.
Classify intentional software purchases, payments for adjacent services, ad spend, stated openness to paid tools, and disputed or unexpected charges separately.
Views, likes, complaints, search volume, competitor prices, and ad spend are not willingness to pay for the proposed product.
Treat self-reported payments as unverified reports, not audited purchases.

Return a concise decision brief and an evidence appendix with up to three opportunities.
For each, explain who has the problem and when, supporting dated excerpts, existing alternatives and the remaining gap, evidence for and against payment, and what remains uncertain.
Recommend one opportunity or state why the evidence is insufficient.
Suggest the smallest experiment before development with a measurable success criterion, preferably an actual payment signal when payment is the open question.
Label proposed prices, recruitment thresholds, and pass criteria as experiment assumptions.
Recommending an experiment does not authorize contacting people, collecting private data, or taking payments.
