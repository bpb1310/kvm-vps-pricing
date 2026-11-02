# linux vps hosting: what to check before you buy, how KVM specials actually price out, and where RackNerd fits in

Most people shopping for linux vps hosting are after the same thing: a cheap machine with full root access that doesn't turn into a problem six months later. The hardware specs are the easy part. What actually separates a good budget VPS from a bad one is renewal pricing, refund policy, and whether the provider's resource promises hold up — and those details usually live in the FAQ or terms page, not on the pricing banner.

This guide walks through the checks worth doing before you order any cheap Linux VPS, then looks at RackNerd, a budget-focused US provider whose current KVM specials start at $21.99 per year — and, more importantly, stay at that price on renewal.

## Quick take

For a personal blog, a small self-hosted app, a proxy or VPN endpoint, or a dev/test box, the sensible default is a **1 GB KVM VPS special at $21.99/year** (about $1.83/month): 1 vCPU, 20 GB SSD, 3 TB monthly traffic, full root, 1Gbps port. If you're running AI tooling like Ollama or AnythingLLM, jump to the 4 GB tier at $59.99/year. Before paying, know this: the specials are annual, and RackNerd's service terms don't offer refunds — so the monthly standard plans are the safer way to test first.

👉 [Check the current RackNerd KVM VPS specials and pricing](https://my.racknerd.com/aff.php?aff=11397&pid=952)

## The full plan list: RackNerd's current KVM VPS specials

RackNerd is currently running five annual KVM VPS specials on its promo page. All of them share the same base package: full root access, 1 IPv4 address, 1Gbps network port, SSD storage, and a choice of deployment locations across North America, Europe, and Asia. Here's the complete lineup as shown on the official specials page:

| Plan | CPU / RAM | SSD | Monthly traffic | Price (annual) | Order |
| --- | --- | --- | --- | --- | --- |
| 1 GB KVM VPS | 1 vCPU / 1 GB | 20 GB | 3 TB | $21.99/yr | [ Order the 1 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=952) |
| 2 GB KVM VPS | 2 vCPU / 2 GB | 35 GB | 5 TB | $35.99/yr | [ Order the 2 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=953) |
| 4 GB KVM VPS | 3 vCPU / 4 GB | 60 GB | 7 TB | $59.99/yr | [ Order the 4 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=954) |
| 6 GB KVM VPS | 6 vCPU / 6 GB | 100 GB | 12 TB | $89.99/yr | [ Order the 6 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=955) |
| 8 GB KVM VPS | 7 vCPU / 8 GB | 150 GB | 20 TB | $119.99/yr | [ Order the 8 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=956) |

A few things worth flagging that don't show up in the comparison columns:

- **Renewal stays at the same price.** RackNerd states on the specials page: "These RackNerd VPS specials are lifetime recurring. You can renew at the same rate for as long as you decide to keep the service." In the budget VPS world, where intro prices often double at renewal, this is the single most consequential line on the page.
- **No refunds.** The service agreement doesn't provide them. Combined with annual billing, this means each special purchase is a twelve-month commitment. Third-party guides covering RackNerd consistently recommend trying a monthly plan for a month or two before locking in a year.
- **OS choices:** CentOS, Rocky Linux, AlmaLinux, Fedora, Debian, or Ubuntu at order time, with reinstalls between distributions available later from the control panel. Custom ISO installs are possible through a support ticket.
- The 1 GB plan is marked "Most popular" on the official page, which matches what it's actually suited for — it's the tier that covers blogs, bots, and lightweight proxies.

## Standard monthly plans: the complete line, for testing before committing

Besides the specials, RackNerd sells a standard KVM VPS line with more storage per gigabyte of RAM, billed month-to-month — which is exactly what you want when you haven't yet verified latency and stability. The full standard line currently looks like this:

| Plan | CPU / RAM | SSD | Monthly traffic | Price | Order |
| --- | --- | --- | --- | --- | --- |
| 512 MB entry | 1 vCPU / 512 MB | 30 GB | 500 GB | $26.99/yr | [ Get the 512 MB entry plan](https://my.racknerd.com/aff.php?aff=11397&pid=1) |
| 1 GB | 2 vCPU / 1 GB | 50 GB | 1 TB | $17.99/mo | [ Order the 1 GB monthly plan](https://my.racknerd.com/aff.php?aff=11397&pid=20) |
| 2 GB | 3 vCPU / 2 GB | 75 GB | 2 TB | $20.59/mo | [ Order the 2 GB monthly plan](https://my.racknerd.com/aff.php?aff=11397&pid=21) |
| 4 GB | 4 vCPU / 4 GB | 130 GB | 3 TB | $24.59/mo | [ Order the 4 GB monthly plan](https://my.racknerd.com/aff.php?aff=11397&pid=22) |
| 6 GB | 5 vCPU / 6 GB | 170 GB | 4 TB | $27.59/mo | [ Order the 6 GB monthly plan](https://my.racknerd.com/aff.php?aff=11397&pid=23) |
| 8 GB | 6 vCPU / 8 GB | 220 GB | 5 TB | $36.59/mo | [ Order the 8 GB monthly plan](https://my.racknerd.com/aff.php?aff=11397&pid=24) |
| 12 GB | 7 vCPU / 12 GB | 300 GB | 6 TB | $55.99/mo | [ Order the 12 GB monthly plan](https://my.racknerd.com/aff.php?aff=11397&pid=25) |

The entry plan is the odd one out: 512 MB of RAM billed annually at $26.99/year rather than monthly, and with the least RAM of anything on this page. It exists for tiny static workloads; anyone running a control panel, Docker, or anything database-backed will feel the 512 MB ceiling immediately, and the 1 GB special at $21.99/year is both cheaper and bigger.

Now the cost comparison, because this is where the two lines diverge hard. Twelve months of the 1 GB annual special cost $21.99 — about $4 more than a single month of the 1 GB standard plan. In other words, if your project survives even six weeks, the annual special has already paid for itself, and it keeps costing a tenth as much for the remaining eleven months. The standard plans buy flexibility and extra disk; the specials buy a drastically lower total cost. Do your homework on latency first (there's a section on that below), then commit annually.

There's also a seasonal angle. RackNerd runs holiday promotions that go below the everyday specials — past Black Friday pricing put a 1 GB plan at $10.60/year, roughly half the regular special price. The catch, according to guides that track these events: limited stock, and popular tiers can sell out within hours on the day. If your timing is flexible, waiting for a holiday window is a legitimate strategy. If it isn't, the everyday specials are the stable fallback.

## What "KVM with full root" gets you — and which plan your workload needs

Virtualization type is the first technical filter when comparing Linux VPS providers. RackNerd uses full KVM virtualization, which means you get your own kernel: Docker, WireGuard, custom systemd services, and self-hosted stacks all run without the restrictions container-based VPS products impose. The Ryzen product line runs on AMD Ryzen 3900X or 7950X hardware with NVMe storage in RAID-10, while the standard KVM line uses Intel Xeon processors with SSD storage.

The practical question is RAM. RackNerd's own documentation gives minimum memory figures for its one-click apps, which double as a decent sizing guide for self-hosting in general:

- **2 GB RAM** handles n8n and Coolify comfortably
- **4 GB RAM** is the floor for Ollama, AnythingLLM, LibreChat, and Hermes Agent
- **8 GB RAM** is required for OpenClaw

So the sizing rule is: decide what you're deploying first, then pick the tier. A blog or lightweight proxy fits in 1 GB. Docker plus an automation tool wants 2 GB. Anything AI-adjacent starts at 4 GB. Disk space is rarely the binding constraint on these plans; RAM is.

Management happens through ctrl, RackNerd's own control panel, included with every special: reboot, OS reinstall, root password reset, one-click app installs, an inbound firewall, and an HTML5 VNC out-of-band console for when SSH breaks or you need to install from your own media. One-click app credentials show up in-panel after deployment. An independent review on VPSBenchmarks (December 2025) timed a sample RackNerd VPS provisioning in 110 seconds, and RackNerd's own ordering guide says to expect the login-information email within 5–15 minutes of payment — so "instant setup" here has numbers behind it from both sides.

👉 [Open the 4 GB KVM VPS special for AI and self-hosted workloads](https://my.racknerd.com/aff.php?aff=11397&pid=954)

## Location choice: test before you order, especially from Asia

RackNerd operates datacenters across roughly twenty locations: Los Angeles, San Jose, Seattle, Utah, Chicago, Dallas, New York, New Jersey, Atlanta, Tampa, Miami, and Ashburn in the US; Montreal and Toronto in Canada; London, Amsterdam, Frankfurt, Strasbourg, and Dublin in Europe; and Singapore in Asia. That list comes from RackNerd's own status page, which currently reports all of them as operational.

For readers connecting from Asia, Los Angeles is the location most often recommended in third-party RackNerd guides, with San Jose as the next candidate — the San Jose facility runs five upstream carriers (NTT, Telia, Hurricane Electric, GTT, Cogent), and NTTrouting tends to be strong toward Asia. A commonly cited test IP for San Jose is 192.210.207.88.

Whichever location you're eyeing, don't trust anyone's latency table, including this one. RackNerd publishes test IPs per location, so ping them from your own connection before ordering — the number you get back is roughly the latency you'll live with. Routes differ meaningfully between ISPs, and a location that benchmarks well for one network can be mediocre for yours. This matters double on the annual specials, since the no-refund policy means you can't cheaply change your mind after the fact.

One reassuring detail about reliability: RackNerd runs hundreds of physical nodes per datacenter, and its public status page reports even single-node failures. When a location shows "Partial Outage," the company explains it usually means one hypervisor out of hundreds, with most customers unaffected. You can find which node your VPS sits on and match it against status updates — a level of transparency you don't always get at this price.

## Where RackNerd is the wrong answer

Being upfront about the limits saves everyone a bad month. RackNerd is an unmanaged, budget-tier service, and the following gaps are documented in independent reviews of it:

- **No enterprise SLA.** Nothing in RackNerd's positioning promises uptime guarantees at the level paid enterprise providers offer. At $21.99/year, some CPU overselling on the specials is to be expected. Fine for personal projects; wrong for a revenue-critical service.
- **DDoS mitigation is not part of the standard package**, and neither are provider-side backups or hourly billing. If your project needs any of those out of the box, budget VPS pricing won't fix the gap. DDoS-prone public services and ephemeral CI workloads both belong elsewhere.
- **IPv6 isn't enabled by default** — it's available but needs to be requested through support.
- **It's unmanaged.** Nobody patches your server. If you can't run apt upgrade on your own, a budget VPS is the wrong product category entirely.

If none of those apply to you, the price-to-package ratio is hard to beat in this bracket — and the locked renewal price is the part that matters most over a two- or three-year horizon. A 1 GB special costs $21.99 in year one and, per the official policy, the same $21.99 in years two and three. Total three-year cost: $65.97. That's the number to compare against competitors' "from $X/month" banners, which usually describe year one only.

## Ordering, payments, and one detail about affiliate links

The order flow, per RackNerd's own ordering guide: pick a plan on the KVM VPS page, then on the configuration screen choose your datacenter, OS, and billing cycle, check out, and pay. Activation is automated; within roughly 5–15 minutes you'll get an order confirmation plus a "KVM VPS Login Information" email containing your IP, SSH root credentials, and ctrl panel address.

One genuine gotcha in that process: your ctrl panel login is separate from your Client Area account. If you lose the panel credentials, the ordering guide points to the "View Email Log" section of your client account to retrieve the original email. Also, if you have any special requirements — a custom ISO, a specific node — open a support ticket after ordering rather than relying on the order notes field.

Payment options per the official blog: PayPal, credit cards, cryptocurrency, and bank wire. Third-party guides also report Alipay support, so if that's your preferred method, confirm the option on the checkout page before assuming.

About clicking through a link like the ones in this article: the tracking system RackNerd's client portal runs on sets a cookie that lasts three months by default, per the platform's documentation. So if you click through, close the tab, and come back next week to finish the order, the attribution still works. No need to complete a purchase in one sitting.

## FAQ

**Are the special prices going to jump at renewal?**
No. RackNerd's specials page states the specials are lifetime recurring — you renew at the same rate for as long as you keep the service. This applies to the annual specials; treat third-party claims about other plan lines with more caution.

**Can I reinstall or switch Linux distributions later?**
Yes. Reinstall anytime from the control panel, and you can move between CentOS, Rocky Linux, AlmaLinux, Fedora, Debian, and Ubuntu freely. Custom ISO installs go through a support ticket, and there's an HTML5 VNC console if you want to install from your own media.

**Can I run multiple VPS on one account?**
Yes. Third-party guides covering RackNerd report there's no limit on how many servers one account can hold.

**What if I'm not sure the service is stable enough?**
Start monthly. The standard KVM line bills month-to-month, and since the specials are non-refundable, one month of testing is the cheapest insurance available. Confirm latency from your location and stability before committing to an annual special.

**How do I know if an outage is affecting me?**
Check RackNerd's public status page. It distinguishes "Partial Outage" (typically a single hypervisor out of hundreds in that location) from "Major Outage" (a whole location, which the company describes as rare), and logs even planned maintenance on individual nodes.

## Before you click order

Match the plan to the workload one more time. Blog, bot, or proxy: the 1 GB special at $21.99/year covers it. Docker with n8n or Coolify: take the 2 GB tier at $35.99/year. Ollama, AnythingLLM, or another AI stack: 4 GB at $59.99/year is the floor, and the official one-click installer handles deployment. Above that, the 6 GB and 8 GB tiers exist for people who already know they need them — most self-hosters don't, at least not in year one.

And run the two-minute checks: ping the test IP of the datacenter you're considering, and if any part of the plan makes you hesitate, buy one month of a standard plan first. When you're ready, the full specials lineup is here:

👉 [See RackNerd's KVM VPS specials and lock in the recurring rate](https://bit.ly/RacKnerd)
