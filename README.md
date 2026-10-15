# BOTANIC CHEMISTRY

**Nature × Science × Everyday.**

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
- Ten sock designs based on the supplied Botanic Chemistry collection board.
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
  app.js                Catalog and shopping interactions
  assets/               Optimized product and campaign images
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

The storefront was inspected at 1440×900 and 390×844. Manual browser checks covered style switching, required-size errors, quantity changes, shipping thresholds, cart persistence, order review, search results and empty search, wishlist filtering, mobile navigation, nested dialogs and Escape dismissal. JavaScript syntax and local asset references were checked separately.

---

<div dir="rtl">

## راهنمای فارسی

این پروژه یک فروشگاه مفهومی جوراب با هویت بصری **Botanic Chemistry** است. رابط وب‌سایت انگلیسی است و مستندات مخزن به دو زبان انگلیسی و فارسی ارائه می‌شوند.

برای راه‌اندازی محلی، توضیح قابلیت‌ها و محدودیت‌های نسخه نمایشی، [راهنمای کامل فارسی](README.fa.md) را بخوانید.

</div>
