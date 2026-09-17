# Sweet Lips

**Where Beauty Meets On The Lips**

A multi-page static website for Sweet Lips, an affordable, trendy, cruelty-free lip care brand based in Durban, South Africa. Founded in 2026, Sweet Lips sells lip gloss, liners, lipsticks, balms, oils, tints, scrubs, masks, care packages, and limited-edition collections.

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Landing page with logo, hero message, "Shop Now!" call to action, and "Why Shop With Sweet Lips" highlights |
| About Us | `about.html` | Brand story, mission, vision, values, and founder bio with photo |
| Products | `products.html` | Full product catalog — 8 individual products with shade/flavor selectors, 3 lip-care packages, and a limited-edition collection |
| Cart | `cart.html` | Shopping cart (static placeholder — empty state only, no cart logic yet) |
| Reviews | `reviews.html` | Customer reviews with star ratings |
| FAQ | `faq.html` | Delivery, cruelty-free policy, and payment method Q&A |
| Contact | `contact.html` | Location, email, WhatsApp, and business hours |
| Socials | `social.html` | Instagram, TikTok, Facebook handles and brand hashtag |

## Brand Details

- **Mission:** To empower everyone to express their confidence through affordable and high quality lip care
- **Vision:** To become South Africa's most loved lip beauty brand while working toward global recognition
- **Values:** Affordability, Inclusivity (shades for every skin tone), Cruelty-Free (no animal testing)
- **Founded:** 2026, by a 19-year-old founder from Durban
- **Delivery:** Nationwide across South Africa, 3–5 business days
- **Payment methods:** Card, EFT, Cash on Delivery
- **Contact:** hello@sweetlips.co.za | WhatsApp 067 144 8554 | Mon–Fri, 9am–5pm
- **Socials:** @sweetlips.sa (Instagram & TikTok), Sweet Lips SA (Facebook), `#SweetLipsSA`

## Product Catalog (from `products.html`)

### Individual Products
| # | Product | Price | Options |
|---|---------|-------|---------|
| 1 | Lip Gloss | R30 | 6 shades (Clear, Baby Pink, Light Pink, Glitter Pink, Nude, Hot Pink) |
| 2 | Lip Liners | R15 | 6 shades (Mauve, Brown Nude, Rose Pink, Berry, Chocolate, Soft Beige) |
| 3 | Lipsticks | R45 | 6 shades (Ruby Red, Nude Pink, Mauve, Coral, Deep Berry, Brown Nude) |
| 4 | Lip Balms | R20 | 6 flavours (Vanilla, Strawberry, Coconut, Cherry, Mint, Mango) |
| 5 | Lip Oils | R50 | 6 shades (Cherry Red, Strawberry Pink, Honey Gold, Coconut Clear, Watermelon Pink, Vanilla Nude) |
| 6 | Lip Tints | R45 | 7 shades (Dark Cherry, Red Berry, Wine, Deep Mauve, Dark Rose, Pink Plum, Rosewood Brown) |
| 7 | Lip Scrubs | R60 | 6 flavours (Pink Sugar, Coffee Brown, Honey Gold, Strawberry Pink, Vanilla Ice Cream, Bubble Gum) |
| 8 | Lip Masks | R50 | Overnight hydration/repair treatment |

### Lip Care Packages
| Package | Price | Contents |
|---------|-------|----------|
| 1 — Mini Pouch Set | R120 | Makeup pouch, overnight lip mask, lip balm, lip brush |
| 2 — Glow Up Set | R180 | Lip scrub, exfoliator brush, overnight sleeping mask, lip balm, mirror |
| 3 — Ultimate Lip Lover Set | R320 | 3 pouches (lips-shaped, clear, toiletry bag) with an assortment of scrubs, masks, and balms inside |

### Limited Edition Lip Collection
| Product | Price | Options |
|---------|-------|---------|
| Metal Applicator Gloss | R35 | 9 shades (Burgundy Cherry, Dark Cherry, Crimson Kiss, Bubble Gum Pink, Grape Pink, Taffy Brown, Rosy Pink, Classic Pink, Chocolate Brown) |
| Color-Changing Lip Gloss | R35 | Color-Changing Pink (natural pink reveal), metal applicator |

## Design & Styling

Styling lives in a single shared stylesheet, `css/style.css`, linked from every page.

- **Palette:** Blush pink and lavender-navy — background `#FFF7FB`, text `#3A3A5C`, accent pink `#FFB6D9` / `#ff6fae`, with page-specific accent shades (e.g. `#c96a8c` on Contact, `#ff4d6d` on FAQ)
- **Fonts:** `Poppins` for body text, `Georgia`/serif for headings
- **Layout:** Centered, card-style `<main>` container with rounded corners and soft box-shadows; a pill-shaped `<nav>` bar; rounded pill-shaped buttons for links inside `<main>`
- **Page-specific classes:** `.cart-page`, `.reviews-page`, `.faq-page`, `.contact-page`, `.social-page` each apply their own accent color and card styling to `<main>`, matching the `<body class="...">` set on each HTML page
- **Image classes:** `.home-pic` (homepage logo), `.about-pic` (circular founder photo with border)
- **Responsive:** Media queries at `768px` and `480px` adjust the nav layout and heading sizes; background image switches from `fixed` to `scroll` attachment on smaller screens for iOS performance
- **Background:** A tinted background image (`images/picc1.jpeg`) is applied site-wide via a white gradient overlay

## Project Structure

```
sweet-lips/
├── index.html
├── about.html
├── products.html
├── cart.html
├── reviews.html
├── faq.html
├── contact.html
├── social.html
├── css/
│   └── style.css
└── images/
    ├── picc1.jpeg                  (site-wide background)
    ├── Logo picture.jpeg
    ├── IMG_1585.jpeg                (founder photo)
    ├── lipgloss collection.jpeg
    ├── lip linerss.jpeg
    ├── neww lipsticks.jpeg
    ├── lip balms.jpeg
    ├── new lip oils.jpeg
    ├── lip tints new.jpeg
    ├── lip scrubs collection.jpeg
    ├── Hydrating Collagen Lip Mask - 20 pack.jpg
    ├── 3 lip care.jpeg              (Package 1)
    ├── 1 lip care.jpeg              (Package 2)
    ├── 2 lip care.jpeg              (Package 3)
    ├── IMG_4006.jpeg                (Metal Applicator Gloss)
    └── limited edition colour changing.jpeg
```


## Tech Stack

- HTML5
- CSS3 (`css/style.css`) — custom styling, responsive media queries, no framework
- No JavaScript yet (needed for a working cart and contact form)

## Contact
Sweet Lips — Durban, South Africa
Email: hello@sweetlips.co.za | WhatsApp: 067 144 8554

## License

&copy; 2026 Sweet Lips. All rights reserved.
## Changelog

### Part 2 Updates
- Added a shared stylesheet (`css/style.css`) and linked it from every page, giving the site consistent colours, fonts, and layout
- Added page-specific styling classes (`.cart-page`, `.faq-page`, `.contact-page`, `.reviews-page`, `.social-page`) for unique accent colours per page
- Expanded `products.html` with shade/flavour selectors, three lip-care packages, and a limited-edition collection section
- Enabled GitHub Pages so the site is publicly viewable via a live link

### Fixes from Part 1 Feedback
- Fixed missing space in `<link rel="stylesheet" href="...">` across 7 pages, which could prevent the stylesheet from loading correctly in some browsers
- Added the missing `viewport` meta tag to 7 pages for proper mobile responsiveness
- Fixed a broken navigation link on the homepage (`product.html` → `products.html`) that caused a 404 error
- Fixed a malformed `<div class="product-card">` around the Lip Scrubs product that was closing itself immediately and breaking the card layout
- Fixed a typo (`<br.` → `<br>`) and missing space in the Lip Scrubs product heading
- Restructured `index.html`: wrapped the page title and navigation in a proper `<header>` tag, removed the deprecated `<center>` element, moved the `<footer>` inside `<body>` (it was previously outside the closing tag), and added the missing `</html>` closing tag
- Moved `style.css` into a `css/` folder to match the path already referenced in the HTML files, fixing a mismatch that caused the site to load with no styling
- ## References

- Google Fonts — Poppins typeface: https://fonts.google.com/specimen/Poppins
- Product images generated using Meta AI
- Claude (Anthropic) — used for code review, debugging assistance, and identifying HTML/CSS issues
- 
