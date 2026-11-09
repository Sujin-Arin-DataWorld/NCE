# NSE STUDIO

**Nature + Science + Everyday**

A concept storefront for NSE STUDIO. The first collection is crew socks. The 2026 Edit adds five individual design-study pages for underwear and socks; boxer briefs and tank tops also appear as generated visual concepts. These studies are not purchasable products.

[English](README.md) · [فارسی](README.fa.md)

An editorial sock storefront built around an ivory, olive and charcoal collection. The interface is English; repository documentation is available in English and Persian.

## Run locally

No installation or build step is required. From the repository root:

```sh
python3 -m http.server 4173 --bind 127.0.0.1 --directory dist
```

Open [http://127.0.0.1:4173](http://127.0.0.1:4173).

If Node.js is installed, the optional shortcuts are:

```sh
npm run dev
npm run check
```

`npm run check` validates JavaScript syntax. It is not a browser or integration test.

## Included

- Full-width editorial campaign and a restrained molecular identity.
- A 2026 Edit on the homepage, with individual detail pages for Flex Micro Brief, Relaxed Boxer, Dawn Rib Crew, Motion Quarter and Low Profile No-show. Each page presents its own image, silhouette, palette and proposed material direction, with clear concept status.
- Ten sock designs, with a new molecular sunrise emblem on the featured Minimal Icon.
- Generated six-color boxer brief and four-color tank top lineups, presented as future product concepts. The boxer waistband pairs one wordmark with one molecular sunrise emblem; tank back print and tag-free inner neck placement are shown in detail mockups.
- NSE STUDIO branding with the Nature + Science + Everyday positioning and a three-part essentials lineup.
- Quick Order with style selection, required size selection, quantity and live price.
- Product details, size and care guides, collection filters, search and wishlist.
- Shopping bag with quantity updates, removal, shipping calculation and order review.
- Browser-local persistence for the bag and wishlist.
- Responsive desktop/mobile layouts, keyboard-operable dialogs and reduced-motion support.

## Project structure

```text
dist/
  index.html            Page markup and dialogs
  styles.css            Responsive design and component states
  concepts.css          2026 Edit and concept detail page styles
  app.js                Catalog and shopping interactions
  assets/               Optimized product and campaign images
  products/             Five static design-study detail pages
.openai/hosting.json    Existing private Sites project configuration
docs/DESIGN.md          Design decisions and asset provenance
README.fa.md           Persian documentation
```

Serve `dist/` on any static web host. The Sites manifest points to the same directory. The project does not require a framework, package installation or a backend.

## Demo boundaries

This is a **concept store**, not a production commerce service. Prices are illustrative USD values. Shipping is illustrated as $5, or free from a $50 subtotal. There is no checkout provider, payment collection, order submission, inventory synchronization or shipping fulfilment. The review screen explicitly states that no order has been placed.

Bag and wishlist data stay in the visitor’s browser. Google Fonts serves Cormorant Garamond and Montserrat. No analytics or connector access is configured.

The photography and collection board are concept assets. Product appearance, fabric specifications, measurements and commercial rights should be confirmed before a real retail launch. See [design and asset notes](docs/DESIGN.md).

## Validation

The 2026 Edit homepage and all five detail pages were rendered in Chromium at 1440×900 and 390×844. All detail routes returned HTTP 200, all five product images loaded, and neither viewport showed document-level horizontal overflow or page errors. The original sock shopping flow was previously checked for style switching, required-size errors, bag updates, order review, search, wishlist and mobile navigation. `npm run check` validates JavaScript syntax.

---

<div dir="rtl">

## راهنمای فارسی

این پروژه یک فروشگاه مفهومی جوراب با هویت بصری **NSE STUDIO** است. رابط وب‌سایت انگلیسی است و مستندات مخزن به دو زبان انگلیسی و فارسی ارائه می‌شوند.

برای راه‌اندازی محلی، توضیح قابلیت‌ها و محدودیت‌های نسخه نمایشی، [راهنمای کامل فارسی](README.fa.md) را بخوانید.

</div>
