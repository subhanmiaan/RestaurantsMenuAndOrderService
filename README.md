<div align="center">

# GOODFILLERS ↗ Motion Edition

**An eight-page restaurant demo with a complete browsing-to-checkout experience.**

Vanilla JavaScript · Responsive layouts · Session-persistent cart · Expressive motion

![HTML](https://img.shields.io/badge/HTML5-Multi--page-3151DF?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-Motion-182459?style=flat-square&logo=css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-No_framework-F7DF1E?style=flat-square&logo=javascript&logoColor=111111)

[Features](#features) · [Quick start](#quick-start) · [Architecture](#architecture) · [Deploy](#deployment)

</div>

## The project

GOODFILLERS is a restaurant website demo by **Muhammad Subhan**. It brings together a substantial menu, cart interactions, delivery/takeaway choices and a consistent visual identity across eight distinct pages.

It is built with plain HTML, CSS and JavaScript. No framework, npm install, API key or database is required. **Checkout is simulated: no order is sent and no payment is processed.**

## Features

| Area | Included behavior |
|---|---|
| Menu | Filters across 15 categories, pizza sizes/crusts and wing portions |
| Cart | Quantity controls, item removal and session persistence between pages |
| Checkout | Delivery/takeaway selection, native form validation and demo order numbers |
| Contact | WhatsApp message preparation; the visitor explicitly sends the draft |
| Gallery | Category filters and image lightbox |
| Reviews | Demo review carousel |
| Navigation | Eight page URLs, mobile menu, order dock and back-to-top control |
| Motion | Page entrances, scroll reveals, parallax, card tilt, button sheen and add-to-bag animation |
| Accessibility | Focus styles, labeled controls, dialog behavior and reduced-motion support |

## Pages

Home `/` · Menu `/menu/` · About `/about/` · Offers `/offers/` · Gallery `/gallery/` · Reviews `/reviews/` · Locations `/locations/` · Contact `/contact/`

Each page has its own HTML file, heading and metadata. A custom 404 page is included.

## Quick start

```bash
git clone https://github.com/subhanmiaan/RestaurantsMenuAndOrderService.git
cd RestaurantsMenuAndOrderService
python3 -m http.server 8000
```

Open **http://localhost:8000**. Python 3 is only used here to serve static files; VS Code Live Server or another static server works too.

## Architecture

| File or directory | Responsibility |
|---|---|
| `index.html` and page directories | Static, pre-rendered page content and shared shell |
| `app.js` | Menu data, reusable page sections, cart, checkout and interactions |
| `style.css` | Responsive layout, visual identity and animation |
| `assets/` | Local restaurant logo and printed menu |
| `vercel.json` | Static output and trailing-slash routing |

Static HTML provides an initial document, then JavaScript enhances the page. Keep page HTML and JavaScript-rendered content in sync when editing shared sections or menu data.

## Deployment

Import this repository into Vercel using **Other**, leave the build command empty, and set the output directory to **`.`**. No application environment variables are needed.

Routes are designed for a **domain root**. Opening through `file://` or publishing unchanged beneath a GitHub Pages repository subdirectory will not resolve root-relative links correctly.

## Demo boundaries

- No food orders, payments or deliveries are transmitted.
- Cart state exists only in the current browser tab session; checkout details are not persisted.
- Demo delivery is **Rs. 150** and takeaway is free. Confirm actual fees and service times before commercial use.
- Reviews, hours and restaurant story include demo content; menu prices come from the supplied printed menu.
- Illustrative photos and Google Fonts require external network access. The local logo is used as an image fallback.
- Social-account ownership and business details need verification before launch.

The supplied contact section uses **2Km Daska Road, Sialkot, Pakistan** and **+92 326 8748721**. These are restaurant content, not the developer’s personal contact details.

## Validation notes

The original implementation records passing JavaScript syntax, route/asset references, page headings/IDs, component rendering and delivery/takeaway calculation checks. A target-device visual review is still recommended; this documentation refresh does not claim a new end-to-end browser test.

## Related projects

- [Stash Pizza](https://github.com/subhanmiaan/RestaurantsMenuAndOrderService2) — a red-and-white adaptation.
- [BuntySajji](https://github.com/subhanmiaan/buntysajji) — a desi menu experience with truck-art accents.

---

Built by [**Muhammad Subhan / @subhanmiaan**](https://github.com/subhanmiaan) · [Contact the developer](mailto:wsubhan5969@gmail.com)
