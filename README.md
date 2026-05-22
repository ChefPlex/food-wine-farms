# sonoma-chef

**Eat well. Drink better. Know where to go.**

This repo is the project home for everything under the Sonoma Chef and Food Wine Farms umbrella - a collection of AI-powered culinary guides I've been building solo since 2025. Regional apps for the App Store. A weekly-updating web guide for Sonoma County. A content pipeline that runs without me touching it. The whole thing started as a side project and became something I'm genuinely proud of.

The short version: I'm a chef, a wine educator, and a Technical Program Manager who lives in Sonoma County. I've spent years at farmers market stalls before the crowds arrive, at winery tasting bars where the pours get more honest after noon, and in professional kitchens where sourcing actually matters. I built these tools because I wanted them to exist, and because I wanted to learn how to build them.

---

## The Projects

### Food Wine Farms
**[foodwinefarms.com](https://foodwinefarms.com) Â· [Projects](https://foodwinefarms.com/projects/)**

The parent brand. Regional culinary guides covering wine country beyond the county line - wherever agriculture, culinary ambition, and a genuine sense of place converge. Locals-first. Honest picks. No filler, no ad relationships, no ranking algorithms.

Nine iOS and iPadOS apps are live on the App Store covering wine country regions across the western U.S. and beyond:

| Region | App Store |
|---|---|
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
**[sonomachef.com](https://sonomachef.com) Â· [Guides](https://sonomachef.foodanddrink.workers.dev/)**

A regional culinary guide for Sonoma County with a web app that updates itself every week without me touching it. Five guide categories, regenerated on a schedule, published to Cloudflare Pages via an automated pipeline running on a cloud Ubuntu server.

| Guide | What It Covers |
|---|---|
| [Weekend Picks](https://sonomachef.foodanddrink.workers.dev/sonoma_chef_WEEKEND.html) | Best dining events, pop-ups, and farmers markets this weekend |
| [90-Day Calendar](https://sonomachef.foodanddrink.workers.dev/sonoma_chef_CALENDAR.html) | Wine dinners, harvest events, festivals - the full season at a glance |
| [Restaurant Roundup](https://sonomachef.foodanddrink.workers.dev/sonoma_chef_restaurant_roundup.html) | Standout tables worth booking now, seasonal picks |
| [The Locals List](https://sonomachef.foodanddrink.workers.dev/sonoma_chef_restaurant_roundup_locals.html) | Weeknight deals, happy hours, prix fixe - eating well without the tourist markup |
| [Farmstands & Markets](https://sonomachef.foodanddrink.workers.dev/sonoma_chef_FARMSTANDS.html) | Where to buy direct from farms - produce, eggs, meat, cheese |

The Sonoma: Food Wine Farms iOS app is also live - same regional depth, native experience on iPhone and iPad.

---

## How It Was Built

Everything here was built solo, with AI tools doing most of the heavy lifting on code I didn't already know how to write. The stack and the approach:

**Content and research** - Claude (Opus and Sonnet), ChatGPT, Grok. Prompt workflows developed to keep content quality consistent across food, wine, and farmstand coverage at scale. The goal was repeatable quality, not one-off drafts.

**App development** - Vibe-coded with Claude Sonnet as the primary tool. I described what I wanted, it wrote the code, I tested and directed. Managed the full App Store submission lifecycle - certificates, provisioning profiles, review process, release - without a development team.

**Web automation** - Cloudflare Pages for hosting, Ubuntu server for the content pipeline, automated weekly publishing. Set it up once, it runs. That was the goal: remove the manual publishing bottleneck so the guides stay current without becoming a second job.

**Content design** - Prompt libraries built specifically for each guide type so the output reads like a person who knows the region, not a summarization of search results.

---

## What I Learned

Building this taught me things that a decade of managing technical programs hadn't - specifically, what it actually takes to ship software as a single person with no team, no budget, and no runway for delay. A few things that stuck:

The hardest part was not the code. It was making the content quality consistent at scale without reviewing every line manually. That's a prompt engineering problem, and it takes more iterations than you'd expect.

Shipping nine App Store apps is mostly an exercise in process management. The code is the easy part. The certificates, the metadata, the screenshots, the review responses, the release cadence - that's where solo developers lose time.

Automation that works is worth ten times the effort to set it up. The weekly pipeline took real work to get right. Now it runs, and I've moved on to the next thing.

AI tools are genuinely useful for solo builders - but only if you treat them as collaborators you have to direct, not oracles you interrogate. The difference between a useful result and a generic one is almost always in the framing.

---

## Status

Active development. New regions are in the works. The content pipeline is running. The iOS apps are live and being updated.

If you're a developer, wine professional, farmer, or food writer in any of the covered regions and you want to talk - the contact is on the sites.

---

## Related Work

This project lives alongside my professional work in technical program management and security. If that side of things is interesting, the TPM repos are here in the same GitHub account.

- [tpm-templates](https://github.com/ChefPlex/tpm-templates) - Program lifecycle templates
- [security-program-playbooks](https://github.com/ChefPlex/security-program-playbooks) - Security program frameworks
- [program-reporting-frameworks](https://github.com/ChefPlex/program-reporting-frameworks) - Reporting and investment frameworks

---

*Eric White - Glass Artist, Chef, Wine Guy, Cat Herder*
*Sonoma County, CA*
