# ShareCanva.com

**Live site: [sharecanva.com](https://sharecanva.com)**

ShareCanva.com is a simple website that shares Canva Pro team invitation links for free. Each period (usually a month), the site publishes a numbered set of 10 Canva Pro invitation links. Visitors pick a link that is still available, open it, and join. That is the whole service: no prices, no orders, no payments, and nothing to sign up for on the site itself.

> **Note:** This repository is documentation only. It describes the website in detail; the source code is private and is not published here. The invitation links themselves are distributed only through the website and are intentionally not listed in this document.

## Why This Exists

Canva Pro team invitations are usually scattered: shared in random posts, buried in comment threads, reposted without any indication of whether they still work, or locked behind groups and paywalls. Anyone looking for a working invitation has to hunt through stale links and guess which ones are still open.

ShareCanva.com was created to give that hunt a single, predictable home. One page, one current period, ten numbered links, each clearly marked as available or full. When a new period starts, the page is updated with a fresh set, and the site states plainly on its own homepage: every link on the page is shared for free.

## Purpose

- Publish free Canva Pro team invitation links in one stable place instead of scattering them across posts and comments.
- Make the state of every link obvious, so visitors do not waste time on invitations that are already full.
- Organize invitations by period (for example, "Canva Pro Bulanan Oktober 2026"), so there is always one clearly current set.
- Keep the experience zero-friction: no accounts, no checkout, no fees.

## Features

- **The current period, front and center.** The homepage opens with the running period (for example, "10 Link Canva Pro Oktober 2026") and a short instruction: pick a link that is still available; it is free and easy to use.
- **Ten numbered invitation links.** Each period offers links numbered 01 to 10, presented as individual entries so visitors can work through them in order.
- **Live availability status.** Every link is labeled with its status, such as "Tersedia" (available) or "Penuh" (full), so a full team never looks the same as an open one.
- **Period archive.** Invitations are grouped by period, and past periods remain addressable through the site's period pages, giving the site a simple history of what was shared and when.
- **Completely free.** As the site's footer puts it, all links on the page are shared for free.

## Frontend

The frontend is a lightweight, content-first website built with Next.js. The homepage is the product: a period title, the numbered list of invitation entries with their status labels, and a short explanation of how to use them. There is no dashboard, no login, and no interactive tooling; the design goal is that a visitor understands the page in seconds and can act on it immediately.

A dynamic period route renders each period's page from the same template, so a new month's set of links looks and behaves exactly like the previous one.

## Backend / How It Works

There is barely a backend, by design:

- The site's content lives in a single configuration data file: the periods, their titles, the ten invitation entries per period, and each entry's availability status.
- Pages are rendered from that data (including the dynamic per-period pages), so updating the site for a new period means updating the data file and redeploying; no database, no admin panel, and no user data of any kind is collected or stored.
- When a team fills up, its entry's status is flipped to full in the same data file, and the next visitors immediately see the correct state.

This static, data-driven setup keeps the site fast, cheap to run, and trivial to maintain, which matters for a free service that is updated on a monthly rhythm.

## Summary

ShareCanva.com is a free, single-purpose page: 10 numbered Canva Pro invitation links per period, each marked available or full, shared openly with no payment and no sign-up. Simple on purpose.

## 🌐 Socials
[![Behance](https://img.shields.io/badge/Behance-1769ff?logo=behance&logoColor=white)](https://behance.net/xsrazy) [![Discord](https://img.shields.io/badge/Discord-%237289DA.svg?logo=discord&logoColor=white)](https://discord.gg/xsrazy) [![Facebook](https://img.shields.io/badge/Facebook-%231877F2.svg?logo=Facebook&logoColor=white)](https://facebook.com/xsrazy) [![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/xsrazy) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/xsrazy) [![Medium](https://img.shields.io/badge/Medium-12100E?logo=medium&logoColor=white)](https://medium.com/@xsrazy) [![Pinterest](https://img.shields.io/badge/Pinterest-%23E60023.svg?logo=Pinterest&logoColor=white)](https://pinterest.com/xsrazy) [![Quora](https://img.shields.io/badge/Quora-%23B92B27.svg?logo=Quora&logoColor=white)](https://quora.com/profile/xsrazy) [![Reddit](https://img.shields.io/badge/Reddit-%23FF4500.svg?logo=Reddit&logoColor=white)](https://reddit.com/user/xsrazy) [![Stack Overflow](https://img.shields.io/badge/-Stackoverflow-FE7A16?logo=stack-overflow&logoColor=white)](https://stackoverflow.com/users/31065073) [![Twitch](https://img.shields.io/badge/Twitch-%239146FF.svg?logo=Twitch&logoColor=white)](https://twitch.tv/xsrazy) [![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?logo=Twitter&logoColor=white)](https://twitter.com/xsrazy) [![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?logo=YouTube&logoColor=white)](https://youtube.com/c/xsrazy)

## 💰 You can help me by Donating
[![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=plastic&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/xsrazy) [![PayPal](https://img.shields.io/badge/PayPal-00457C?style=plastic&logo=paypal&logoColor=white)](https://paypal.me/xsrazy) [![Patreon](https://img.shields.io/badge/Patreon-F96854?style=plastic&logo=patreon&logoColor=white)](https://patreon.com/Xsrazy) [![Ko-Fi](https://img.shields.io/badge/Ko--fi-F16061?style=plastic&logo=ko-fi&logoColor=white)](https://ko-fi.com/xsrazy)
