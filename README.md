# GOODFILLERS — Motion Edition

A complete eight-page restaurant demo made by Subhan / @subhanmiaan.

## Pages

Home, Menu, About, Offers, Gallery, Reviews, Locations and Contact. Each has its own URL, HTML file, heading and search/social metadata. A custom 404 page is included.

## Source

Plain HTML, CSS and JavaScript. No framework, build command, npm install, API key or database is required. Shared behaviour is in `app.js`; responsive styles and animation are in `style.css`. Page HTML is pre-rendered for immediate content and graceful no-JavaScript browsing, then enhanced by the shared script. Editable menu and section components live in `app.js`; keep static page HTML in sync when changing content.

## GitHub and Vercel

Upload the contents of this folder to the root of a GitHub repository. Import that repository into Vercel. Use the Other preset, leave the build command empty, and use `.` as the output directory. The supplied `vercel.json` configures the output directory and trailing-slash page URLs.

For local use, serve this folder using VS Code Live Server or another static web server. Root-relative page links are designed for hosting at a domain root, not opening files directly through file:// or a GitHub Pages repository subdirectory.

## Features

- Menu filtering across 15 categories, pizza sizes/crusts and wing portions.
- Delivery and takeaway with cart quantity controls and session persistence between pages.
- Native form validation and simulated checkout with demo order numbers.
- WhatsApp message preparation; visitor explicitly sends the message in WhatsApp.
- Gallery filters/lightbox, review carousel and full-screen mobile navigation.
- Cinematic page entrances, scroll reveals, desktop image parallax, subtle card tilt, button sheen, add-to-bag animation, page transitions and mobile order dock.
- Keyboard focus states, native accessible dialogs and reduced-motion support.

## Demo boundaries

No payments are processed and no food orders are sent. The cart is stored only in the visitor's current browser tab session. Personal checkout details are not persisted. Reviews, hours and restaurant story are demo content. Menu prices are based on the supplied printed menu. Delivery is Rs. 150; takeaway is free.

Logo and printed menu are bundled in `assets`. Illustrative food/lifestyle photos load from external image hosts; Google Fonts also require an internet connection. Local logo fallback handles image-load errors. Social account ownership is not verified.

Address: 2Km Daska Road, Sialkot, Pakistan.
Phone / WhatsApp: +92 326 8748721.
Credit: Made by @subhanmiaan.

## Validation

JavaScript syntax, page-component rendering, route/local-asset references, unique page headings and IDs, and delivery/takeaway calculation checks passed. Visual browser testing was not available in the authoring environment.
