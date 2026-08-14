# Pedestal — US Market Opportunity

A 26-month snapshot of **US demand** (almost entirely organic) across all 11 Pedestal Shopify
storefronts (Jun 2024 – Jul 2026). Pedestal has no US-localized store and no
US-targeted ad spend, yet US visitor sessions are substantial and growing fast.
Bot & AI-agent traffic is flagged out so the headline reflects **real people**.

## Start here
Open **`index.html`** in any browser — it's the one-page summary with the
animated maps, growth chart, top markets, and method notes.

## The numbers (real customers, bots/AI agents removed)
- **172,506** real US visitor sessions over 26 months
- **+71% year-over-year** (last 12 months vs the prior 12: ~104,000 vs ~60,700 sessions); a log-linear trend implies ≈64%/yr
- **~9,000 real sessions/month** at the current rate (Jun 2026: 9,222 · Jul 2026: 8,921)
- Top states: **California (31.9k) › New York (20.7k) › Texas (15.0k) › Washington › Florida › Illinois**
- Top cities: **Los Angeles › New York › Brooklyn › San Jose › Chicago › Fort Worth › San Antonio › Seattle**
- California + New York + Texas ≈ **39%** of US demand

## What's in the box
```
index.html                     One-page opportunity summary (open this)
maps/
  states-by-month.html   Interactive animated state choropleth (also embedded in index.html)
  cities-by-month.html   Interactive animated city bubble map (top metros)
charts/
  overview.html / overview.png     Real humans vs bots/AI agents; growth + top markets
data/
  real-customers_state-by-month.csv   Real-customer sessions by state × month
  real-customers_city-by-month.csv    Real-customer sessions by city × month
  all-traffic_state-by-month.csv      All sessions incl. bots/AI agents (for reference)
  all-traffic_city-by-month.csv       All sessions incl. bots/AI agents (for reference)
```
The maps are interactive and embedded in `index.html`; the charting library loads
from a CDN, so viewing needs an internet connection.

## Method & the bot/AI caveat
- **Source:** Shopify "Sessions by location" report, all 11 storefronts, United
  States only, monthly. Figures are **website sessions (visits), not orders.**
- **Why filter bots/AI agents:** ~50% of raw "US sessions" originate from cloud
  datacenters — Council Bluffs IA (Google), Ashburn VA (AWS), North Bergen NJ,
  Forest City NC (Meta), Prineville OR. These are search/AI crawlers, on-demand
  AI fetchers (ChatGPT, Perplexity, Google AI) and uptime/monitoring bots. They
  geolocate to the **server**, not a person, so including them would put the
  "market" wherever Amazon/Google/Meta keep their servers (it makes Iowa and New
  Jersey outrank California). They're excluded from the real-customer view and
  preserved in the `all-traffic_*` files.
- **The filter follows the bots.** During 2026 the older hubs went quiet and new
  ones ramped up, mostly Meta's newer datacenter sites. The exclusion list was
  extended in Aug 2026 — Social Circle GA, Gallatin TN, DeKalb IL, Huntsville AL,
  Eagle Mountain UT (all Meta), plus Hillsboro OR, St Louis MO, Columbus OH,
  Springfield NE, Sandston VA — and re-applied to the full series so every month
  is stated on the same basis (this trimmed previously published history by ~3%).
  New datacenter towns are identified by an even session spread across all 11
  storefronts (real US visitors concentrate heavily on the EN-language stores)
  plus a step-ramp from near zero.
- **AI-driven *human* visits are still counted.** When a person reads a ChatGPT
  or Google-AI answer that cites Pedestal and clicks through, that's a normal
  session at their real location — already in the real-customer numbers.
- Mixed metro/datacenter cities (e.g. Fort Worth TX, Des Moines IA) are kept in
  the real-customer view when the store-mix looks predominantly human; a finer
  user-agent-level split remains a logical next step.

*Prepared June 2026 · updated August 2026 · data through July 2026.*
