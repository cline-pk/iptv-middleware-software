# IPTV Middleware Software (Self-Hosted, One-Command Install)

**IPTV middleware software** is the layer between your video streams and your subscribers. It signs users in, decides what each one may watch, sends the channel list and the TV guide (EPG), and connects billing. Without middleware you have streams, but no service.

[Xtream-Masters](https://xtream-masters.com/iptv_middleware.php) is a self-hosted IPTV and OTT middleware for operators: one secure Go binary that runs on your own Ubuntu servers and also manages streams, load balancers and resellers.

## Install in one command

Run as root on a clean Ubuntu server (18.04 to 26.04, 24.04 recommended):

```bash
curl -fsSL -o xm-install https://iptv-admin.xtream-masters.com/cms_install/xm-install && chmod +x xm-install && ./xm-install
```

Setup takes about 2 to 5 minutes. Full guide: [IPTV middleware software](https://xtream-masters.com/iptv_middleware.php).

## What IPTV middleware does

| Job | In Xtream-Masters |
|---|---|
| Sign-in and devices | User lines, ActiveCode (one code, one device), MAG and Stalker portal, Enigma2 |
| Packages | Bouquets decide which channels, movies and series each subscriber gets |
| TV guide | EPG with automatic matching, catch-up and TV archive |
| Billing | Multi-tier resellers with credits and payment gateways (Stripe, PayPal, Coinbase, Cryptomus, Binance) |
| APIs | Admin API, Reseller API, Player API (Xtream Codes compatible), ActiveCode API |
| Scale | Unlimited load balancers on one license, optional Multi-Main edge servers |
| Hosting | Your own Ubuntu servers, 18.04 to 26.04 |

## Types of IPTV middleware software

| | Enterprise suite | Cloud (SaaS) middleware | Self-hosted panel (Xtream-Masters) |
|---|---|---|---|
| Typical buyer | Telecoms, hotels, campuses | New OTT brands without servers | IPTV and OTT providers with resellers |
| Where it runs | On-premise or vendor cloud | Vendor cloud | Your own Ubuntu servers |
| Pricing model | Quote, often per subscriber | Monthly fee, often per user tier | Flat monthly license |
| Manages streams and servers | Usually a separate product | Usually included, on vendor servers | Yes, with unlimited load balancers |
| Reseller billing | Rarely | Sometimes | Yes, multi-tier with credits |
| Time to start | Weeks to months | Days | One command, about 2 to 5 minutes |

## How to choose IPTV middleware software

1. **Devices your customers use.** Android and Fire TV apps, Smart TVs, MAG boxes, Enigma2, web. The middleware must sign in every one of them.
2. **Who owns the servers and the data.** Cloud middleware runs on the vendor servers. Self-hosted middleware runs on yours.
3. **Pricing as you grow.** Per-subscriber pricing rises with every customer. A flat license stays the same.
4. **Reseller and billing support.** Resellers need their own panel, credits and payment gateways.
5. **APIs.** Look for an Admin API, a Reseller API and an Xtream Codes compatible Player API, so existing IPTV apps work.
6. **Scaling and security.** Load balancer limits, edge servers, connection limits per user, protected stream links.

## Price

EUR 40 per month until 31 December 2026, EUR 70 per month from 1 January 2027, for the main server and unlimited load balancers.

## Coming from Xtream UI, XUI.ONE, NXT or 1-Stream?

Migration is supported. See the [IPTV panel migration guide](https://github.com/cline-pk/iptv-panel-migration-guide).

## FAQ

**What is IPTV middleware?**
The software between the video streams and the subscriber. It signs users in, applies their package, sends the channel list and TV guide, and links to billing.

**IPTV middleware vs IPTV panel?**
Same core job. Telecoms and hotels say middleware and usually mean an enterprise suite. IPTV and OTT providers say panel and mean self-hosted software that also manages streams, load balancers and resellers.

**Can I self-host IPTV middleware software?**
Yes. Xtream-Masters installs on your own Ubuntu server with the command above.

## Links

- [IPTV middleware software](https://xtream-masters.com/iptv_middleware.php)
- [IPTV panel](https://xtream-masters.com/iptv_panel.php)
- [IPTV server software](https://xtream-masters.com/iptv_server_software.php)
- [Player API documentation](https://xtream-masters.com/guide/xtream_codes_api_player_api_documentation.php)
