# Webshare pricing: per-GB rates, per-IP plans, and whether the free tier is enough

Type "webshare pricing" into a search bar and you get three numbers that refuse to agree with each other: $2.99 a month, $7 per GB, and free. All three are real. They just belong to different products sold on two different meters, and that mismatch is why people close the pricing page convinced Webshare is either a steal or a trap.

The split is simple once you see it. Webshare rents datacenter proxies and static residential (ISP) addresses per IP, per month. It sells rotating residential traffic per gigabyte. Renting a shared datacenter address and buying a gigabyte of traffic through someone's home connection are not comparable purchases, so any article that lines up "$0.03/IP" next to "$3.50/GB" and declares a winner is comparing two different things.

Below is what each product actually costs, what the headline numbers hide, and where the per-GB side of the bill stops looking competitive.

## The free plan, since that's what most people come for

Webshare gives every new account 10 shared datacenter proxies with up to 1 GB of bandwidth a month. No credit card, no countdown, and it renews rather than expiring — it's a permanent tier, not a trial that quietly converts into a charge. PCMag's review notes the free tier limits your location choices to Japan, Spain, the UK and the United States, and that the non-US pools are thin.

1 GB a month is a few thousand page loads on a light site. That's enough to point a scraper at your real target once and find out whether proxies solve your problem at all. It is not a production tier, and 10 shared datacenter IPs will fold the moment a target starts filtering datacenter ranges.

## Webshare datacenter pricing: the cheap meter, and it is genuinely cheap

The datacenter product — Webshare calls it "Proxy Server" in the dashboard — is priced per IP per month, with a bandwidth allowance folded in (250 GB on the standard tiers). Shared 100 proxies is the smallest paid plan at **$2.99/month**. Volume drops the unit price hard:

| Proxies | Monthly per IP | Yearly per IP | Monthly total |
| --- | --- | --- | --- |
| 100 | $0.0299 | $0.0239 | $2.99 |
| 1,000 | $0.0269 | $0.0215 | $26.90 |
| 5,000 | $0.0239 | $0.0191 | $119.50 |
| 60,000 | $0.0179 | $0.0144 | $1,074.00 |

Two things worth flagging. First, Webshare advertises "save 30%" for annual billing, but on the per-proxy products the yearly per-IP figure and the yearly total shown on the page don't divide evenly — at 100 proxies the yearly rate works out closer to $0.0199/IP once you divide the advertised total by the count. Second, the "from $0.018/IP" line on the homepage is the 60,000-proxy tier. At the 100-proxy entry point you're paying roughly 1.7× that.

For undefended targets — internal tools, public APIs, small sites, SEO rank checks, geo-testing your own properties — this ladder is hard to beat on price, and 250 GB of included bandwidth covers a lot of small requests.

## Rotating residential: per GB, and this is the meter that decides budgets

Residential is the only Webshare product billed by traffic, and the ladder is steep in both directions:

| Monthly bandwidth | Price per GB |
| --- | --- |
| 1 GB | $3.50 |
| 10 GB | $2.75 |
| 25 GB | $2.60 |
| 50 GB | $2.45 |
| 100 GB | $2.25 |
| 250 GB | $2.00 |
| 500 GB | $1.75 |
| 1,000 GB | $1.50 |
| 3,000 GB | $1.40 |

The listed rack rate is $7.00/GB, and a standing 50% discount is applied automatically at checkout — no coupon needed. That's worth knowing for two reasons. Your real entry price is $3.50/GB, not $7, but the discount is still a promotion, so the number moves if it ever lapses. Annual billing takes another 30% off exactly on this product: $3.50/GB monthly becomes $2.45/GB yearly, and the 100 GB tier drops from $2.25 to $1.58.

Two structural details matter more than the discounts. Webshare's residential plans are monthly subscriptions that auto-renew, not balances you draw down; a month you don't use is a month you paid for, and unused bandwidth doesn't roll over. And the residential pool is claimed at 80M+ IPs across 195 countries, against 400K+ datacenter IPs — vendor figures, worth treating as vendor figures.

## Static residential (ISP): the flat-rate quirk nobody mentions

Static residential proxies come from real ISP ranges, hold the same address, and are billed per IP per month, usually with unlimited bandwidth. Webshare starts at **$0.30/IP for 20 proxies** ($6/month) and steps down slowly: roughly $0.285/IP at 500, $0.27 at 1,000, and $0.225 at 10,000 ($2,250/month).

Here's the part that catches people: the per-IP rate is flat from the 20-IP minimum all the way to 250 IPs. Buying 40 addresses instead of 20 saves you nothing per unit. Volume discounts only kick in at 500. Buy the count you need and stop optimizing. Webshare also sells private and dedicated versions of both static residential and datacenter at higher per-IP rates, for when a neighbour's traffic patterns become your problem.

## What a month of Webshare actually costs, by workload

Sticker prices blur once you apply them. Four realistic shapes:

**Rank tracking or light scraping, 10 GB of residential a month.** $2.75 × 10 = **$27.50/month**. On yearly billing the same tier runs about $19.25/month equivalent.

**A mid-sized scraper, 100 GB a month.** $2.25 × 100 = **$225/month** on monthly billing, roughly $157.50/month equivalent yearly.

**1,000 datacenter proxies for a self-hosted tool.** $26.90/month, with bandwidth included.

**Three terabytes of residential a month.** $1.40 × 3,000 = **$4,200/month** at the best published rate.

That last row is the one to sit with. Webshare's per-GB curve only becomes cheap at volumes that most teams never reach, and reaching them means committing to a monthly subscription whether or not the traffic gets used.

## Where the per-GB pricing stops making sense

Everything above treats datacenter as the value product and residential as the expensive one. That's how Webshare's own lineup works out. The free plan is a datacenter product, the sub-three-cent IPs are datacenter, and the per-GB product behind the "$7/GB" headline is the one where the price argument gets thin.

If your monthly residential usage is unpredictable — a burst of scraping in March, nothing in April, a client project in June — a subscription metered per month is the wrong shape regardless of the rate. That's the gap pay-as-you-go providers built their business on.

One of them is worth pricing alongside, and it's the one this page links to. DataImpulse sells the same traffic on a per-GB, pay-as-you-go basis with no subscription: residential at **$1/GB**, datacenter at $0.50/GB, mobile at $2/GB, premium residential at $5/GB. Bought gigabytes never expire, so a quiet month costs nothing instead of costing a full month's subscription.

👉 [see DataImpulse's current per-GB pricing](https://bit.ly/dataimPulse)

Its full lineup, as published:

| Plan | Entry package | Rate | Volume tiers | Billing model |
| --- | --- | --- | --- | --- |
| Residential | $5 / 5 GB | $1.00/GB | $0.80/GB at 1 TB, $0.70/GB at 5 TB | [grab the residential starter pack](https://bit.ly/dataimPulse) |
| Datacenter | $5 / 10 GB | $0.50/GB | $50 / 100 GB, $450 / 1 TB ($0.45/GB), custom from $2,250 for 5 TB+ | [pick a datacenter tier](https://bit.ly/dataimPulse) |
| Mobile (4G/5G/LTE) | $5 / 2.5 GB | $2.00/GB | $50 / 25 GB, $1,600 / 1 TB ($1.60/GB), custom from $8,000 for 5 TB+ | [check the mobile plan](https://bit.ly/dataimPulse) |
| Premium residential | $5 / 1 GB | $5.00/GB | $50 / 10 GB, custom from $20,000 for 5 TB+ | [view premium residential](https://dataimpulse.com/premium-residential-proxies/?aff=86938) |

Side by side, the arithmetic on residential is blunt. 100 GB with Webshare is $225/month. The same 100 GB at DataImpulse costs $100 one time, and whatever you don't burn stays in the account. At a terabyte, Webshare's best published rate works out to $1,500 for the month against $800 for a non-expiring terabyte. Webshare's plan includes 80M+ residential IPs and its own routing stack; DataImpulse claims 90M+ IPs across 195 countries, a 99.51% success rate, HTTP/HTTPS and SOCKS5, rotating and sticky sessions (sticky runs 1–120 minutes, defaulting to 30), country targeting included, and city/ZIP/ASN targeting billed at double the standard residential rate.

The honest counterpoint: this is not a slam dunk in every direction. If what you actually need is 100 or more static datacenter addresses for undefended targets on a predictable monthly bill, Webshare's per-IP ladder beats per-GB pricing comfortably — a hundred proxies for $2.99 with 250 GB included is not a number DataImpulse's $0.50/GB datacenter tier can match for that shape of work. The comparison flips on usage pattern, not on brand.

## Picking between the two meters

- **Testing whether proxies work at all:** Webshare's free tier costs nothing and needs no card. DataImpulse's $5/5 GB entry gets you real residential IPs for a one-off five dollars, which is a different kind of low-risk.
- **Lots of cheap static datacenter IPs, steady monthly use, unguarded targets:** Webshare's datacenter ladder. Nothing else in this price range comes close per address.
- **One fixed IP that looks like a home connection, per account:** static residential or ISP, priced per IP on both models.
- **Bursty, hard-target scraping where monthly volume swings:** per-GB pay-as-you-go. Paying a subscription for idle months is the expensive version of this workload.
- **A fixed monthly residential volume you always burn:** the subscription discount curve is real, and at 3,000 GB the $1.40/GB rate is a genuine bargain — as long as you actually use it every month.

👉 [compare the pay-as-you-go plans before you commit to a subscription](https://bit.ly/dataimPulse)

## Fine print worth reading before you buy

Webshare doesn't offer free trials on its paid products; the free tier is the only way to test without paying. There's a 48-hour refund window subject to usage caps — up to 1 GB of bandwidth on the proxy server and static residential products. The company was acquired by Oxylabs in 2022 and continues to operate independently under that umbrella, which is relevant if you were planning to shortlist Webshare and Oxylabs as two separate options.

On the DataImpulse side, the refund window for new users is listed at seven days, support is 24/7 and human rather than a bot queue, and advanced targeting on residential multiplies the per-GB rate by two, so a city-level campaign costs more per gigabyte than the headline $1/GB suggests. Budget for that before you scale.

## Questions people actually ask

**Is Webshare's free plan really free?** Yes. Ten shared datacenter proxies, up to 1 GB of traffic a month, no credit card, no expiry date, and it doesn't auto-convert to a paid plan.

**So how much does Webshare cost?** Between $2.99/month for 100 shared datacenter proxies and $4,200/month for three terabytes of residential. The single "starting at" figure on the homepage is $0.018/IP, which is the 60,000-proxy tier, not the entry price you'll see at checkout.

**Is Webshare cheaper than DataImpulse?** On datacenter addresses, yes — Webhare's per-IP model wins for bulk static IPs. On residential bandwidth, no: $3.50/GB at the entry tier against $1/GB pay-as-you-go, with the further catch that Webshare's traffic is subscription-metered and doesn't roll over while DataImpulse's never expires.

**Do unused Webshare gigabytes carry over?** No. Residential is billed as a monthly subscription, so a month you don't use is a month you've paid for.

**Why does Webshare advertise $0.018 per IP if I'll pay $0.0299?** Because both are real, just at different volumes. $0.018/IP arrives at 60,000 proxies. The 100-proxy plan is $0.0299/IP, and the advertised floor is a volume figure quoted as a starting price — common practice across the proxy market, rarely spelled out.

The short version: Webshare pricing is two products wearing one price tag. Read the meter before you read the number, and you'll know within a minute whether you want the cheapest IPs on the market or cheaper residential gigabytes.
