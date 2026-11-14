# Akile JPPro: ¥24.99/Month Starting Price, Six Plans, and the 10Mbps Throttle Explained (Full Plan Table)

Akile JPPro is the Tokyo VPS line Akile sells to people who need workable latency from mainland China: three-network optimized routing, ports up to 1.2Gbps, and DNS-based unlocking of Japanese streaming catalogs. Monthly pricing runs from **¥24.99 for JPPro-Light to ¥447.50 for JPPro-Ultra**, across six tiers. None of them cut you off when the monthly traffic allowance runs out; the port drops to a shared 10Mbps and the server keeps serving.

Most buyers end up choosing between Standard at ¥62.25 and Pro at ¥122.50. The two cheapest tiers look like better deals than they are, for a reason that has nothing to do with the price tag, and that's covered below along with the full table, the real annual cost, and what the routing tests actually show.

> **Quick picks**
> - Testing streaming, running a tiny site, low monthly volume → JPPro-Light at ¥24.99/month
> - Normal site hosting, a few devices, headroom on the port → JPPro-Standard at ¥62.25/month
> - Need 2GB RAM plus a larger allowance → JPPro-Pro at ¥122.50/month
> - Team workloads, sustained transfers, multiple services → JPPro-Max or JPPro-Ultra
>
> 👉 [Check the current JPPro plan lineup and stock](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811)

## Akile JPPro plans and prices

| Plan | vCPU / RAM / Disk | Traffic | Port | Price/month | Order |
| --- | --- | --- | --- | --- | --- |
| JPPro-Light | 1 / 1GB / 10GB | 700G | 300Mbps | ¥24.99 | [Check JPPro-Light price](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| JPPro-Starter | 1 / 1GB / 20GB | 500G | 1000Mbps | ¥37.35 | [Check JPPro-Starter price](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| JPPro-Standard | 1 / 1GB / 20GB | 1024G | 1200Mbps | ¥62.25 | [Check JPPro-Standard price](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| JPPro-Pro | 1 / 2GB / 20GB | 2048G | 1200Mbps | ¥122.50 | [Check JPPro-Pro price](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| JPPro-Max | 2 / 2GB / 20GB | 3072G | 1200Mbps | ¥248.75 | [Check JPPro-Max price](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |
| JPPro-Ultra | 4 / 4GB / 20GB | 5120G | 1200Mbps | ¥447.50 | [Check JPPro-Ultra price](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811) |

Every plan ships with one IPv4 and one IPv6 address by default.

Traffic figures need a caveat. The Light, Starter, Standard and Pro numbers above come from a March 2026 plan listing. Max and Ultra were re-checked on 4 November 2026 and confirmed at 3072G and 5120G. Some older write-ups circulating for this series list 1TB to 8TB per month across the board, which is two to four times higher than what the plan pages show, so don't budget from a review's table. Take the figure from the order page on the day you buy.

## What the six tiers actually change

Three things move as you go up: RAM, disk, and port speed. Traffic moves too, and not monotonically.

Light and Starter are the odd pair. Starter costs ¥12.36 more per month and gives you a 1000Mbps port instead of 300Mbps, but its monthly allowance is **500G against Light's 700G**. You are paying for port speed and a second 10GB of disk, and handing back 200G of traffic. Anyone whose workload is mostly downloading or streaming should notice that. Anyone pushing burst traffic through a fast pipe will prefer Starter.

Standard is the first tier with the full 1200Mbps port and a 1024G allowance, still on 1 core and 1GB RAM. Pro keeps the same port and disk but doubles RAM to 2GB and traffic to 2048G. Max doubles cores to 2 and adds another 1024G. Ultra goes to 4 cores and 4GB RAM with 5120G.

RAM is the real jump. Between Standard and Pro you are paying roughly double for 1GB of extra memory and twice the traffic. If a 1GB box with a small database or a couple of Docker containers is already swapping, Pro fixes that. If it isn't, Standard carries you a long way for ¥62.25.

## What a year actually costs

Multiply the monthly price by twelve and you get the honest baseline: Light ¥299.88, Starter ¥448.20, Standard ¥747.00, Pro ¥1,470.00, Max ¥2,985.00, Ultra ¥5,370.00.

Akile publishes annual pricing for only two tiers on the current listing:

- **JPPro-Max annual: ¥2,487.50**, which is 10 × the ¥248.75 monthly rate. Against twelve monthly payments of ¥2,985, that saves ¥497.50.
- **JPPro-Ultra annual: ¥4,475.00**, or 10 × ¥447.50. That saves ¥895 against ¥5,370.

In both cases you pay for ten months and get twelve. It's a straightforward 16.7% reduction, worth taking if you're confident you'll stay a year. For Light, Starter, Standard and Pro, no annual price is published in the listings checked, so don't assume the same 10-for-12 math applies. Confirm at checkout whether an annual option exists for those tiers at all.

👉 [Open the JPPro order page to compare monthly and annual totals](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811)

## The 10Mbps throttle, in practical terms

When the monthly allowance is exhausted, bandwidth is capped at a shared 10Mbps. Nothing is suspended and no overage invoice appears. At 10Mbps you can still serve a text-heavy site, run SSH, push a backup, or keep a monitoring agent alive. You cannot stream 4K or move a 50GB archive in an afternoon.

If you need full speed back before the billing cycle resets, traffic can be reset for a fee that scales with the plan: ¥22 on Light, ¥17.50 on Starter, ¥35 on Standard, ¥70 on Pro, ¥105 on Max, ¥175 on Ultra. Note that Starter's reset is cheaper than Light's, which tracks the smaller allowance on Starter.

The practical read is that these are metered plans with a soft floor rather than hard caps, and the reset prices tell you what Akile expects each tier to consume. On Standard, one reset costs more than half the monthly fee, so a workload that needs two resets a month belongs on Pro.

👉 [Check the current JPPro Standard price and reset options](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811)

## Routing and measured performance

JPPro runs on KVM with AMD EPYC hosts. A third-party test of a 1.2Gbps JPPro configuration recorded an EPYC 7402P at 2797MHz, 1 core, 1GB RAM, BBR enabled, disk I/O around 342MB/s, and an IP geolocated in Tokyo. Average ping from tested mainland locations came in around 74ms. The same write-up called the disk I/O weak relative to the CPU, which matches the numbers: 342MB/s is fine for a web front end and unremarkable for anything I/O-bound.

The routing is where the marketing and the traceroutes diverge, so read carefully:

- **Unicom** outbound goes AS4837 direct to Tokyo, then hands over to IIJ into the facility. Return traffic leaves via Japan SoftBank and connects back to AS4837.
- **Mobile** outbound goes CMI direct to Hong Kong, then IIJ to Tokyo. The return path from the facility is hidden before it hands off to CMI.
- **Telecom** outbound rides the 163 backbone direct to Tokyo, then IIJ. The return leg from the facility is also hidden before rejoining 163.

All three outbound paths are backbone direct to Tokyo followed by IIJ. Return paths are not uniform: Unicom comes back over SoftBank, the other two are partially hidden. This is a solid China-optimized route set, not a premium end-to-end product, and it should not be described as CN2 GIA or as a single high-end line in both directions. If your users are mostly on Unicom, the return path is the most clearly documented of the three.

## DNS unlock, and where it stops

JPPro is advertised as supporting DNS unlock for Japanese streaming services. That is a DNS-level redirect to an unlocking resolver. It is not a native Japanese IP, and the plan page makes no promise about Netflix, Disney+, ChatGPT or anything else specifically. Akile's JPHyper node is the one that explicitly lists Netflix, Disney+, YouTube, ChatGPT, Abema and DMM.

So treat JPPro as suitable for Japanese catalog access where a DNS unlock is enough, and unsuitable where the service fingerprints the IP itself. If native IP matters to your use case, this isn't the product, and no amount of plan upgrades changes that.

## Who should skip JPPro

Three groups:

**Anyone who needs native IPs.** Covered above. DNS unlock won't substitute.

**Anyone serving a US or European audience.** JPPro is built around mainland China latency into Tokyo. Akile's own positioning points China-focused buyers at its Hong Kong, Japan, Korea and Singapore locations and away from US and European ones.

**Anyone shopping purely on price.** ¥24.99/month is the entry point, but it buys a 300Mbps port and 700G. If you just want a cheap box somewhere in Asia, Akile's other Japan lines start lower; JPHyper-Lite was listed at ¥14.99/month and JPHyper-One at ¥7.30/month in March 2026 data, though those figures may have moved. Those aren't China-optimized the way JPPro is. Within the same brand, JPIIJ-Lite sat at ¥24.99/month with a 1000Mbps port and a 1000G allowance in the same March listing, which is a different trade: more port speed, no three-network optimization claim.

Also worth flagging: in March 2026, Light and Starter were both marked sold out and Standard showed five units left. That stock snapshot is long stale, but the pattern is real. The cheap tiers are the ones that disappear first.

## Ordering

The path on Akile's site is: select Type as Traffic-Based Cloud Server, then Region as Japan, then pick the JPPro node you want. Supported images include Debian 11 and 12, Ubuntu 18, 20 and 22, and RockyLinux 8 and 9. Payment goes through Alipay, WeChat Pay or PayPal, and much of the catalog is priced in CNY, which keeps card conversion fees out of the picture for Chinese buyers.

Two things the public pages don't answer: refund terms and whether any discount code is active. A March 2026 listing noted no code available at that time, which says nothing about today. Confirm both with support before paying if either matters to you.

## Picking one

Match the plan to the bottleneck, not to the price you'd like to pay:

- Streaming checks and a small site → **Light**, accepting the 300Mbps port and 700G.
- Burst traffic through a fast pipe → **Starter**, accepting 500G.
- A normal site, a few services, 1GB RAM is enough → **Standard**.
- Already swapping on 1GB, or moving 2TB a month → **Pro**.
- Multiple containers, a team, sustained transfers → **Max**, and take the annual price if you're staying.
- Heavy multi-core work alongside high traffic → **Ultra**.

Before checkout, verify two numbers on the order page: the traffic allowance for the specific tier, since published figures have varied across listings, and whether an annual option exists for anything below Max. Those two checks are worth more than any review table, including this one.

👉 [Start from the JPPro plan page and confirm today's traffic allowance](https://akile.io/register?aff_code=24a6f6bd-f995-4158-a9fd-f4b6aef27811)
