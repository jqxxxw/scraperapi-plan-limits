# Web Data Extraction Tools: Which Type Fits Your Job, What 1,000 Pages Really Costs, and Where ScraperAPI's $49 Plan Stops Being Enough

Web data extraction tools split into three jobs that barely overlap: getting data off web pages, pulling fields out of documents like invoices and ID cards, and syncing records between SaaS apps and a warehouse. Choosing the wrong one of those three costs far more time than choosing the wrong brand inside the right one.

ScraperAPI belongs to the first group. It's a scraping API: you send a URL, it returns HTML or parsed JSON, and it handles proxies, JavaScript rendering and bot-protection bypass for you. The entry paid tier is **Hobby at $49/month for 100,000 credits and 20 concurrent threads**, and there's a 7-day trial with 5,000 credits that doesn't ask for a card.

Below: every ScraperAPI plan as listed on its pricing page, what a credit actually buys on different sites, what the same $49 turns into as you move up tiers, and which job type each category of tool handles better.

> **Quick pick.** A few thousand pages a month, code-friendly workflow, want a stable API instead of a browser: Hobby at $49/month covers 100,000 standard requests. Past roughly 100,000 standard pages a month, jump to Startup at $149/month, which cuts the per-page cost about 3x. Most people never need anything above Business.
> 👉 [Check current ScraperAPI plan prices and credit allowances](https://www.scraperapi.com/pricing/?fp_ref=coupons)

## Every ScraperAPI plan, side by side

| Plan | Credits per month | Concurrent threads | Price (monthly billing) | Get it |
| --- | --- | --- | --- | --- |
| Free | 1,000 | 5 | $0 | [Start on the free plan](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Hobby | 100,000 | 20 | $49/mo | [Open Hobby](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Startup | 1,000,000 | 50 | $149/mo | [Open Startup](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Business | 3,000,000 | 100 | $299/mo | [Open Business](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Scaling | 5,000,000 | 200 | $475/mo, or $427.50/mo billed annually | [Open Scaling](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Professional | 10,500,000 | 300 | Custom quote | [Request Professional pricing](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Advanced | 21,500,000 | 500 | Custom quote | [Request Advanced pricing](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Enterprise | 22,000,000+ | 500+ | Custom quote | [Talk to sales](https://www.scraperapi.com/pricing/?fp_ref=coupons) |

Two things in that table decide more purchases than the credit counts do.

Geotargeting is limited on the cheap tiers. Hobby and Startup can target the US and EU only. Country-level targeting starts at Business, and it costs no extra credits once you have it.

Analytics history is capped at the last 30 days on Hobby and Startup, and unlimited from Business up. If you're debugging why a selector broke three weeks ago, that difference matters.

Annual billing takes exactly 10% off any tier. On Scaling that's $5,130/year instead of $5,700, and you can renew early to pull a fresh batch of credits rather than waiting out the month.

## What one credit buys, and why $49 goes 25x further on some sites

A standard page costs 1 credit. Almost nothing else does. ScraperAPI prices by domain difficulty and by which features you switch on, and the multipliers stack onto the base cost.

| Request type | Credits | Pages from Hobby's 100,000 credits |
| --- | --- | --- |
| Standard page | 1 | 100,000 |
| Amazon, Walmart, eBay | 5 | 20,000 |
| Google or Bing, including subdomains | 25 | 4,000 |
| LinkedIn | 30 | 3,333 |
| JavaScript rendering (`render=true`) | 10 | 10,000 |
| Bot-protection bypass (Cloudflare, DataDome, PerimeterX, Akamai) | +10 | ~9,000 |
| Premium proxy (`premium=true`) | 10 | 10,000 |
| Screenshot (`screenshot=true`) | 10 | 10,000 |
| Ultra premium (`ultra_premium=true`, paid plans only) | 30 | 3,333 |

Geotargeting, sticky sessions, device type, output format and auto parsing add nothing to the cost. The Domain Cost Estimator in the dashboard gives the exact figure for any specific URL, and `max_cost` lets you cap a single request so a surprise domain can't burn through a day's credits.

That multiplier is why "how much does it cost per page" has no single answer. Price it per plan and per target:

| Plan | Per 1,000 standard pages | Per 1,000 Amazon pages | Per 1,000 Google searches |
| --- | --- | --- | --- |
| Hobby ($49) | $0.49 | $2.45 | $12.25 |
| Startup ($149) | $0.15 | $0.75 | $3.73 |
| Business ($299) | $0.10 | $0.50 | $2.49 |
| Scaling ($475) | $0.095 | $0.48 | $2.38 |

The gap between Hobby and Scaling is about 5x on plain pages. On Google searches the same two plans differ by roughly 5x as well, but the absolute numbers are 25 times higher, so a SERP-heavy job that looks affordable on paper can eat a Business plan in a week. Run your actual mix through the table before you pick a tier. This is the single most common sizing mistake with credit-based scrapers, and it's arithmetic, not opinion.

👉 [Compare the Hobby and Startup credit allowances against your page count](https://www.scraperapi.com/pricing/?fp_ref=coupons)

## Pick by job type, not by brand

### Web pages

The hard part of web scraping stopped being extraction years ago. It's access: JavaScript-rendered content, Cloudflare and DataDome, login walls, IP rate limits, and selectors that break when a layout changes. Tools in this category differ mostly in how much of that they absorb for you.

| Tool | Where it fits | Verified entry price | Watch out for |
| --- | --- | --- | --- |
| ScraperAPI | URL in, HTML or JSON out, with proxy rotation and bypass handled | $49/mo (Hobby, 100,000 credits) | Credit multipliers on hard domains; no LLM schema extraction |
| Octoparse | Five or more sites, no code, template-driven | Free (10 tasks, 50K rows/mo, local runs only), Standard $69/mo billed annually | Cloud runs need Standard or above |
| Apify | Scraping inside an existing codebase | Free ($5/mo credit), Starter $29/mo, Scale $199/mo, Business $999/mo | Many Actors add per-result fees on top of compute |
| Bright Data | Enterprise anti-bot targets at volume | From $1.50 per 1,000 results (pay-per-result) | Different product lines use different pricing, so compare like with like |
| Firecrawl | LLM and RAG pipelines needing Markdown or schema JSON | Free, paid from $19/mo; Standard $99/mo for 100,000 credits | A JSON scrape costs 5 credits per page |

Octoparse is the least technical route if your targets are popular sites: 600+ templates cover Amazon, Google Maps, LinkedIn, Indeed, Yelp and Zillow, and there's an MCP server for ChatGPT, Claude, Cursor and Gemini. Its free plan runs locally only, so anything scheduled or running overnight needs a paid tier.

Firecrawl is the one to look at if the output goes into a model rather than a spreadsheet. It returns clean Markdown or schema-defined JSON, handles JavaScript automatically, is open source and self-hostable, and goes up to 150 concurrent requests. Its credit math is aggressive on structured output: a `/scrape` call with a JSON schema costs 5 credits per page, so the $99 Standard tier's 100,000 credits is 20,000 extracted pages, not 100,000.

Apify suits developers who want a marketplace of ready-made scrapers (1,500+ Actors, Playwright and Puppeteer underneath, full REST API even on the free tier). Budget carefully, because per-result Actors stack fees on top of platform compute.

Bright Data is the option for targets that fight back hard: 400M+ proxy IPs across 195 countries, dedicated Unlocker and SERP APIs, up to 5,000 URLs per request and a 99.99% uptime claim. Its published entry rate of $1.50 per 1,000 results is pay-per-result, which is a different billing model from a monthly credit subscription, so don't line the two numbers up directly.

ScraperAPI's niche is narrower and clearer: you have URLs, you want HTML or parsed JSON back, and you don't want to maintain a browser fleet. It covers rotating proxies including premium residential and mobile IPs, JavaScript rendering, CAPTCHA and anti-bot bypass, automatic retries, 15-minute sticky sessions and unlimited bandwidth. Structured-data endpoints return parsed JSON for Amazon, Walmart, eBay, Home Depot, Google (Search, News, Jobs, Shopping, Maps) and Redfin. The Async API handles batch jobs with callbacks, and DataPipeline takes up to 100,000 URLs, keywords or ASINs per project from a form, CSV or webhook and outputs HTML, JSON or CSV on a schedule. MCP, LangChain, LlamaIndex, n8n and Zapier integrations exist, though there's no LLM-powered "give me these fields from any page" extraction, which is exactly where Firecrawl earns its place.

### Documents

Invoices, receipts, purchase orders, passports and bank statements need OCR and layout understanding, not proxies. Docparser starts at $39/month with a 30-day trial and uses anchor-based zonal OCR, which suits fixed-format paperwork. Rossum handles handwritten and multi-language documents across 276+ languages with a 14-day trial and custom pricing. Nanonets does zero-shot custom extraction with a free tier that scales into paid quickly. Apache Tika is the free, self-hosted option if you only need text and metadata out of PDFs, Office files and archives, with no AI extraction at all.

None of these will scrape a product page, and ScraperAPI won't read an invoice. Budget for two tools if you need both.

### Databases

Moving SaaS records into Snowflake, BigQuery or Redshift is an ETL problem. Fivetran runs about $120/month with 500+ managed connectors and a 14-day trial. Airbyte is open source and free to self-host, with cloud from $10/month and 350+ connectors. Hevo charges $239/month with 1M free events monthly and real-time CDC. Skyvia starts at $79/month and adds reverse ETL.

If your destination is a spreadsheet, skip this category entirely.

## The limits that decide whether you finish the job

ScraperAPI's free plan is a test environment, not a small production plan. **1,000 credits a month is 1,000 standard pages, 200 Amazon pages, 40 Google searches or 33 LinkedIn pages**, at 5 concurrent threads. That's enough to validate a parser on one site. It is not enough for anything on a schedule.

Then there's the overflow behaviour, which is where plan sizing gets real. Credits reset at each renewal and unused ones are lost, so buying a bigger annual plan doesn't bank capacity for a busy quarter. Run out and scraping pauses until renewal by default. Exceed your thread limit and requests come back as HTTP 429 rather than being queued or billed.

Pay-as-you-go is available on **Scaling, Professional, Advanced and Enterprise only**, at a fixed per-credit rate up to a monthly cap you set. On Hobby, Startup and Business, the alternative is auto-upgrade, which is opt-in and moves you to the next tier when credits run out. This creates a cliff worth planning around: if a job needs 1.1M credits, Startup's 1M won't stretch and there's no overflow to buy, so you're on Business at $299 instead of Startup at $149. Trim rendering to the pages that need it, set `max_cost`, and leave headroom.

The pattern shows up across the category. Octoparse's own analysis of users who signed up in 2025 and 2026 found paid users were roughly four times as likely as free users to run jobs in the cloud, and cloud reliability (scheduled retries, error alerting, handling for schema drift) is the line between a trial and a production workflow. Free tiers finish one-off pulls. They rarely finish recurring ones.

👉 [Start the 7-day trial with 5,000 credits, no card required](https://www.scraperapi.com/pricing/?fp_ref=coupons)

## FAQ

**Is the free plan enough to finish a project?**
For a one-time pull of under 1,000 standard pages on a single site, yes. For recurring jobs, multi-site crawls, or anything hitting Amazon, Google or LinkedIn, no: 200 Amazon pages or 40 searches per month disappears fast.

**What actually changes between 20 and 200 concurrent threads?**
Threads cap how many requests are in flight at once. Moving from Hobby's 20 to Scaling's 200 widens that pipe tenfold, which matters for time-boxed work like a nightly refresh across 500,000 URLs. It doesn't change your credit allowance, so a high-thread plan with a small credit pool still runs dry.

**Do I need to write code?**
The core product is an API endpoint that takes a URL plus parameters, so yes for the main path. DataPipeline is the low-code alternative: form, CSV or webhook in, HTML, JSON or CSV out, on a schedule, up to 100,000 URLs per project.

**Can it render JavaScript and get past Cloudflare?**
Yes, at a credit cost. `render=true` is 10 credits, bot-protection bypass adds 10 when ScraperAPI activates it, and premium proxies are another 10. `max_cost` caps any single request so an awkward domain can't run away with your balance.

**Does it return JSON, or only HTML?**
Both. Output format and auto parsing cost nothing extra, and the structured-data endpoints return parsed JSON for Amazon, Walmart, eBay, Home Depot, Google properties and Redfin. What it doesn't do is LLM-based extraction against an arbitrary schema on any page.

**ScraperAPI, Firecrawl or Bright Data?**
Firecrawl if the output feeds a model and you want Markdown or schema JSON without preprocessing. Bright Data if you need residential IP volume and per-result pricing against heavily defended sites. ScraperAPI if you want predictable per-domain credit costs on a URL-to-HTML/JSON API and don't need AI extraction.

## Which one to buy

Match the tool to the job first, then the plan to the page count.

- Under 1,000 pages, one time: free tier, or open source (Beautiful Soup for HTML, Crawl4AI for Markdown, Apache Tika for documents). Your cost is time, not money.
- 1,000 to 100,000 standard pages a month with code involved: Hobby at $49. If most pages need rendering, treat your real ceiling as 10,000 pages, not 100,000.
- Above 100,000 standard pages: Startup at $149. The per-page price drops from $0.49 to $0.15 per 1,000.
- Multi-site, no code: Octoparse Standard at $69/month billed annually, since cloud runs aren't on the free plan.
- Above 5M credits or unpredictable spikes: Scaling at $475/month, the cheapest tier with pay-as-you-go and a spending cap.
- Documents or warehouse syncs: a separate tool, whichever category your data lives in.

Three things to confirm before you enter a card anywhere. The ScraperAPI trial takes no card, so it doesn't roll into a charge, and when it ends you land on the 1,000-credit free plan rather than a paid tier. Annual billing is exactly 10% off monthly and credits don't carry over between renewals, so don't overbuy to "stock up". And check whether your plan has overflow at all, because below Scaling, running out means your job stops.

👉 [Pick the ScraperAPI plan that matches your monthly page volume](https://www.scraperapi.com/pricing/?fp_ref=coupons)
