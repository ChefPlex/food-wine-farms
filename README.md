# food-wine-farms

**Eat well. Drink better. Know where to go.**

This repo is the project home for everything under the Sonoma Chef and Food Wine Farms umbrella - a collection of culinary guides I've been building solo since 2025. Regional apps for the App Store. A weekly-updating web guide for Sonoma County. A content pipeline that runs without me touching it.

The short version: I'm a chef, a wine educator, and a Technical Program Manager who lives in Sonoma County. I've spent years at farmers market stalls before the crowds arrive, at winery tasting bars where the pours get more honest after noon, and in professional kitchens where sourcing actually matters. The knowledge behind these guides is real - what the AI does is help me produce it at a scale and speed I couldn't match writing everything by hand. The curation is mine. The judgment calls are mine. The tools just handle the volume.

I built these because I wanted them to exist, and because I wanted to learn how to build them.

---

## The Projects

### Food Wine Farms

**[foodwinefarms.com](https://foodwinefarms.com) & [Projects](https://foodwinefarms.com/projects/)**

The parent brand. Regional culinary guides covering wine country beyond the county line - wherever agriculture, culinary ambition, and a genuine sense of place converge. Locals-first. Honest picks. No filler, no ad relationships, no ranking algorithms.

Nine iOS and iPadOS apps are live on the App Store covering wine country regions across the western US and beyond:

| Region | App Store |
|--------|----------|
| Sonoma County | [Sonoma Food Wine Farms](https://apps.apple.com/us/app/sonoma-food-wine-farms/id6761626016) |
| Napa County | [Napa County Food Wine Farms](https://apps.apple.com/us/app/napa-county-food-wine-farms/id6763771134) |
| Mendocino County | [Mendocino Co Food Wine Farms](https://apps.apple.com/us/app/mendocino-co-food-wine-farms/id6764890326) |
| Sierra Foothills | [Sierra Foothills Food Wine Farms](https://apps.apple.com/us/app/amadoreldorado-food-wine-farms/id6762565386) |
| Santa Cruz | [Santa Cruz Food Wine Farms](https://apps.apple.com/us/app/santa-cruz-food-wine-farms/id6762024101) |
| Monterey County | [Monterey Co Food Wine Farms](https://apps.apple.com/us/app/monterey-co-food-wine-farms/id6762565396) |
| Paso Robles | [Paso Robles Food Wine Farms](https://apps.apple.com/us/app/paso-robles-food-wine-farms/id6762007493) |
| Willamette Valley | [Willamette Val Food Wine Farms](https://apps.apple.com/us/app/willamette-val-food-wine-farms/id6762567887) |
| Finger Lakes | [Finger Lakes Food Wine Farms](https://apps.apple.com/us/app/finger-lakes-food-wine-farms/id6762152124) |

Each app covers restaurants, wineries, farmstands, and seasonal events for its region. Paid products. Shipped solo.

---

### Sonoma Chef

**[sonomachef.com](https://sonomachef.com) & [Guides](https://sonomachef.foodanddrink.workers.dev/)**

A regional culinary guide for Sonoma County with a web app that updates itself every week without me touching it. Five guide categories, regenerated on a schedule, published to Cloudflare Pages via an automated pipeline running on a cloud Ubuntu server.

| Guide | What It Covers |
|-------|---------------|
| [Weekend Picks](https://sonomachef.foodanddrink.workers.dev/sonoma_chef_WEEKEND.html) | Best dining events, pop-ups, and farmers markets this weekend |
| [90-Day Calendar](https://sonomachef.foodanddrink.workers.dev/sonoma_chef_CALENDAR.html) | Wine dinners, harvest events, festivals - the full season at a glance |
| [Restaurant Roundup](https://sonomachef.foodanddrink.workers.dev/sonoma_chef_restaurant_roundup.html) | Standout tables worth booking now, seasonal picks |
| [The Locals List](https://sonomachef.foodanddrink.workers.dev/sonoma_chef_restaurant_roundup_locals.html) | Weeknight deals, happy hours, prix fixe - eating well without the tourist markup |
| [Farmstands and Markets](https://sonomachef.foodanddrink.workers.dev/sonoma_chef_FARMSTANDS.html) | Where to buy direct from farms - produce, eggs, meat, cheese |

The Sonoma: Food Wine Farms iOS app is also live - same regional depth, native experience on iPhone and iPad.

---

## How It Was Built

Everything here was built solo, with AI tools doing most of the heavy lifting on code I didn't already know how to write. The distinction worth making: AI handles the production volume. The underlying expertise is mine.

**Content and curation** - The guides are grounded in real knowledge of these regions - years of eating, drinking, shopping at farmstands, and knowing which winery pours honestly and which farmers market vendor actually grows what they're selling. That context is what makes the prompts produce something useful rather than generic. Prompt workflows were developed specifically for each guide type to keep quality consistent at scale. The goal was repeatable quality that reads like a person who knows the region, not a summarization of search results. Because it is.

Tools used for content: **ChatGPT** for research and initial drafts, **Claude Opus and Sonnet** for long-form content, refinement, and prompt development, **Grok** for image generation across the apps and guides.

**App development** - Vibe-coded primarily with **Claude Sonnet** and **Claude Code (CLI)** - I described what I wanted, it wrote the code, I tested and directed. **Claude Cowork** for iterative session work. Managed the full App Store submission lifecycle - certificates, provisioning profiles, review process, release - without a development team. Nine apps shipped this way.

**Web automation** - Cloudflare Pages for hosting, Ubuntu server for the content pipeline, automated weekly publishing. Set it up once, it runs. The goal was to remove the manual publishing bottleneck so the guides stay current without becoming a second job.

---

## Quality Control

Current-event, venue, and seasonal information goes stale fast. The pipeline helps keep the guides moving, but it does not get the final vote.

AI helps with scale. It does not decide what belongs in the guide. The prompts work because they start from real local knowledge: regions I know well, sourcing patterns I care about, and the difference between a useful recommendation and something that reads like a tourism board produced it. Anything that reads generic, outdated, or venue-list-without-judgment gets rewritten or cut.

Guides are reviewed through a mix of source checks, local knowledge, automated refreshes, and manual spot checks. The human review is not a nice-to-have. It is what separates a useful guide from a plausible-looking one that sends people to a restaurant that closed in 2023.

---

## What I Learned

Building this taught me things that a decade of managing technical programs hadn't - specifically, what it actually takes to ship software as a single person with no team, no budget, and no runway for delay.

The hardest part was not the code. It was making the content quality consistent at scale without reviewing every line manually. That is a prompt engineering problem, and it takes more iterations than you'd expect. The difference between a useful result and a generic one is almost always in the framing - and the framing requires knowing what good actually looks like.

Shipping nine App Store apps is mostly an exercise in process management. The code is the easy part. The certificates, the metadata, the screenshots, the review responses, the release cadence - that is where solo developers lose time.

Automation that works is worth ten times the effort to set it up. The weekly pipeline took real work to get right. Now it runs, and I've moved on to the next thing.

AI tools are genuinely useful for solo builders - but only if you treat them as collaborators you have to direct, not oracles you interrogate. Domain knowledge is the multiplier. Without it, you get plausible-sounding content that a local would immediately recognize as wrong.

---

## Status

Active development. New regions are in the works. The content pipeline is running. The iOS apps are live and being updated.

If you're a developer, wine professional, farmer, or food writer in any of the covered regions and want to talk - contact is on the sites.

---

## Related Work

This project lives alongside my professional work in technical program management and security. If that side of things is interesting, the TPM repos are here in the same GitHub account.

- [tpm-templates](https://github.com/ChefPlex/tpm-templates) - Program lifecycle templates
- [security-program-playbooks](https://github.com/ChefPlex/security-program-playbooks) - Security program frameworks
- [program-reporting-frameworks](https://github.com/ChefPlex/program-reporting-frameworks) - Reporting and investment frameworks

---

*Eric White - Glass Artist, Chef, Wine Guy, Cat Herder | Sonoma County, CA*

## License

Copyright (c) 2026 Eric White. Licensed under [CC BY 4.0](LICENSE): use it, adapt it, put it to
work in your own program. Credit is the only condition.
