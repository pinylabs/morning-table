# Morning Table

> **Preview: the full template is being built by the Pinies.** This repository is a small working EmDash site: its home page is the accepted design, and the rest is EmDash's own `marketing-cloudflare` template. The Pinies' real build lands here later.

A calm, photo-led EmDash site for a neighbourhood café: one picture, a short menu and Book a table.

## Start it

- **In Piny:** pick it in the Templates tab.
- **Outside Piny:** `npm create astro -- --template github:pinylabs/morning-table`, then `pnpm install` and `pnpm dev`, and open `/_emdash/admin` to set up the site.

It needs Node 22 or later and pnpm. On Cloudflare it uses a D1 database (`DB`) and an R2 bucket (`MEDIA`), as EmDash's Cloudflare templates do.

## Photos

They are linked from their sources and never copied into this repository. Every page credits them in its footer.

- The home's hero, first of three; the About page: [Keghan Crossland](https://unsplash.com/@keghancphoto) on Unsplash, [Unsplash License](https://unsplash.com/license), linked from [its page](https://unsplash.com/photos/modern-coffee-shop-interior-with-curved-counter-ZZxmc66SjfM), not copied.
- The home's hero, second; the About and Visit pages: [Aleksandra Dementeva](https://unsplash.com/@alexphotogram) on Unsplash, [Unsplash License](https://unsplash.com/license), linked from [its page](https://unsplash.com/photos/long-wooden-table-with-chairs-in-a-modern-room-K8fPaxVDJyU), not copied.
- The home's hero, third; the Menu page: [Joe Hepburn](https://unsplash.com/@thatjoebloke) on Unsplash, [Unsplash License](https://unsplash.com/license), linked from [its page](https://unsplash.com/photos/cup-of-cappuccino-EcWFOYOpkpY), not copied.
- The home's bakery band; the Bakery page: [Conor Brown](https://unsplash.com/@commonboxturtle) on Unsplash, [Unsplash License](https://unsplash.com/license), linked from [its page](https://unsplash.com/photos/a-bunch-of-croissants-that-are-on-a-table-sqkXyyj4WdE), not copied.

The footer's credits for the other pages come from `src/utils/credits.ts`; keep it in step with the seed's photos.

## Styling

Tailwind CSS 4. The design tokens (colours, fonts, type scale, spacing, widths, radii) are in `src/styles/theme.css`, the one file to edit to retheme the site; `src/styles/global.css` holds the dark variant, the base styles and the few components. Motion is calm and stops under `prefers-reduced-motion`.

## Licence

MIT. The Piny Studio mark in `public/brand/` is Piny's and isn't covered by the MIT licence. Built on EmDash's `marketing-cloudflare` template, MIT, Copyright 2026 Cloudflare Inc.; its notice is kept in [LICENSE](LICENSE). Made by the Pinies in [Piny](https://piny.studio/home/).
