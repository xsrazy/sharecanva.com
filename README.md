# ShareCanva.com

A simple website that shares Canva Pro team invitation links for free. Each period, usually a month, the site publishes a numbered set of 10 invitation links, each marked as available or full.

**Live:** https://sharecanva.com

> This is a documentation (showcase) repository. The website's source code is private and lives in a separate repository. The invitation links themselves are distributed only through the website and are intentionally not listed here.

## About

Canva Pro team invitations are usually scattered across random posts and comment threads, with no indication of whether they still work. ShareCanva.com gives them a single, predictable home: one page, one current period, ten numbered links with a clear status on each. There are no prices, no orders, no payments, and nothing to sign up for on the site itself.

## Features

- The current period front and center, for example "10 Link Canva Pro Oktober 2026", with a short instruction to pick a link that is still available
- Ten numbered invitation links per period (01 to 10), presented as individual entries visitors can work through in order
- Live availability status on every link: "Tersedia" (available) or "Penuh" (full)
- Each period gets its own page through the site's dynamic period route, so past periods stay addressable
- Completely free, as the site itself states: all links on the page are shared for free

## Architecture

- Frontend: a lightweight, content-first website built with Next.js. The homepage is the product: a period title, the numbered invitation entries with their status labels, and a short explanation. No dashboard, no login, no interactive tooling
- Routing: a dynamic period route renders each period's page from the same template, so a new month's set of links looks and behaves exactly like the previous one
- Backend: barely any, by design. No database, no admin panel, and no user data is collected or stored

## How It Works

1. All content lives in a single configuration data file: the periods, their titles, the ten invitation entries per period, and each entry's availability status
2. Pages are rendered from that data, including the dynamic per-period pages
3. When a team fills up, its entry's status is flipped to full in the data file, and the next visitors immediately see the correct state
4. Updating the site for a new period means updating the data file and redeploying

## Notes

- Status check (23 October 2026): all ten links of the October 2026 period are currently marked "Penuh" (full) on the live site

## License

MIT License. See [LICENSE](LICENSE) for details.
