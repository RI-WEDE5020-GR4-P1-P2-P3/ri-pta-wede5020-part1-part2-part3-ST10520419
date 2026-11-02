# The Scent Plug Website — Part 3

**Student:** Otlotleng Mogomotsi  
**Student number:** ST10520419  
**Module:** WEDE5020 — Web Development (Introduction)

## About

This is the Part 3 continuation of The Scent Plug website. It keeps the existing black, white and gold style and adds JavaScript interactions, search and sorting, working client-side cart behaviour, form validation, SEO information and a general service-area map.

The Part 2 mark supplied was **83/100**. The mark sheet showed the total but did not identify which criteria lost marks. This Part 3 changelog therefore records the new work completed from the Part 3 brief; it does not claim specific Part 2 corrections that were not shown in the feedback.

## Pages

- `index.html` — homepage and featured products
- `shop.html` — searchable, filterable and sortable product list
- `product.html` — product details (supports `?id=fresh-breeze`, `?id=sweet-desire`, `?id=classic-scent`, or `?id=perfumed-roll-on`)
- `about.html` — business information
- `faq.html` — expandable FAQ answers
- `enquiry.html` — product, price, availability and delivery enquiry form
- `contact.html` — contact form and general service-area map
- `cart.html` — cart quantity updates and removal
- `checkout.html` — order summary and order request form

## Run locally

1. Extract the ZIP file.
2. Open the folder in Visual Studio Code.
3. Open `index.html` with Live Server, or open it directly in a browser.
4. The Leaflet map needs an internet connection to load map tiles. Other main pages and interactions work locally.

## Features added for Part 3

- Responsive mobile navigation, CSS transitions, hover/focus states and reduced-motion support.
- Product cards are rendered from `js/products.js`.
- Shop search, product-type filter, price/name sorting and result count.
- Product detail selection through URL query strings.
- Lightbox for product images and quick-view dialogs.
- Accessible FAQ accordions.
- Interactive Leaflet map with OpenStreetMap attribution. The marker describes a general Mmakau/Ga-Rankuwa service area, not an exact business address.
- Cart stored in browser local storage, with quantity changes, remove buttons, totals and a checkout summary.
- Enquiry and contact forms with required fields, browser validation, message length limits and clear response messages.
- Order, enquiry and contact details are compiled into an email draft using the visitor's email application.
- Unique page titles, meta descriptions and keyword metadata, structured headings, descriptive image filenames and alt text.
- `robots.txt` and `sitemap.xml` are included. Replace the example site URL in `sitemap.xml` after choosing the final deployment address.

## Important setup before publishing

1. In `js/site.js`, replace `thescentplug@gmail.com` with the real business email. Update the sample email and telephone number shown in `contact.html` and in the FAQ.
2. The forms prepare an email draft using `mailto:`. The customer must press **Send**. This static website does not include a server or email service, so it does not send messages automatically.
3. Replace the example URL in `sitemap.xml` with the final GitHub Pages or hosting URL, then submit the sitemap to search engines if desired.
4. The checkout is an order request only. It does not take card details or process payment.
5. Confirm the real service area and delivery policy before publishing.

## Project structure

```text
The_Scent_Plug_Part3/
├── index.html
├── shop.html
├── product.html
├── about.html
├── enquiry.html
├── contact.html
├── faq.html
├── cart.html
├── checkout.html
├── robots.txt
├── sitemap.xml
├── README.md
├── CHANGELOG.md
├── css/style.css
├── js/products.js
├── js/site.js
├── assets/images/
└── screenshots/             # Part 2 responsive screenshots supplied
```

## Deployment with GitHub Pages

1. Create or use your WEDE5020 GitHub repository and copy all files from this folder into it.
2. Commit in clear stages, for example: `Add Part 3 page metadata and navigation`, `Add product search and cart interactions`, `Add validated enquiry and contact forms`, `Add map, sitemap and project documentation`.
3. In GitHub, open **Settings → Pages**, choose the `main` branch and `/ (root)` folder, then save.
4. Update `sitemap.xml` with the published URL. Add the repository URL and published site URL to your learning management submission.
5. Capture new screenshots of the Part 3 website at desktop, tablet and mobile widths. The included screenshots are the Part 2 evidence and should not be presented as Part 3 evidence.

## References

- The Independent Institute of Education. 2026. *WEDE5020 Web Development (Introduction): Part 3 — Enhancing Functionality and SEO* (activity brief supplied for this project).
- MDN Web Docs. *HTML: HyperText Markup Language*. Available at: https://developer.mozilla.org/en-US/docs/Web/HTML (Accessed: 1 November 2026).
- MDN Web Docs. *CSS: Cascading Style Sheets*. Available at: https://developer.mozilla.org/en-US/docs/Web/CSS (Accessed: 1 November 2026).
- MDN Web Docs. *JavaScript*. Available at: https://developer.mozilla.org/en-US/docs/Web/JavaScript (Accessed: 1 November 2026).
- Leaflet. *Leaflet — an open-source JavaScript library for mobile-friendly maps*. Available at: https://leafletjs.com/ (Accessed: 1 November 2026).
- OpenStreetMap contributors. *Copyright and attribution*. Available at: https://www.openstreetmap.org/copyright (Accessed: 1 November 2026).
- Product photographs and screenshots: supplied with The Scent Plug website project.
