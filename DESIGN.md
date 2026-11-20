---
name: Kisetsu Spa
source: https://www.figma.com/design/eZ3CZRNYdN59jArgGQjgjo/Kisetsu-Website (Page 1 > Web Design)
frames:
  desktop: KisetsuSpa_Website_UI_Desktop (1440 x 5952)
  mobile: KisetsuSpa_Website_UI_Mobile (440 x 6343)
colors:
  primary-green: '#405b3d'
  primary-lightgreen: '#cee6cc'
  offer-green: '#dfeddd'
  winter-white: '#bbcdd7'
  summer-yellow: '#d2d386'
  placeholder-gray: '#d9d9d9'
  white: '#ffffff'
typography:
  family: Roboto Condensed (Google Fonts, 300/400/500/700/800)
  card-title: 80px ExtraBold, line-height 1 (mobile 60px)
  card-subtitle: 30px Regular (mobile 24px)
  card-desc: 24px Regular (mobile 20px)
  card-intro: 20px Regular, light green (mobile 18px)
  price: 60px ExtraBold, line-height 0.95; duration 24px Medium
  fine-print: 12px Light, line-height 1.1
  hero: 42px Regular, line-height 1.1, light green, mix-blend lighten (mobile 32px)
  nav: 20px Light, active item Bold
  footer-heading: 32px Regular, light green; phone 32px Bold white
---

# Kisetsu Spa design system

Recreated from the Figma file above. Values in `index.css` `:root` match the Figma variables (`primary-green`, `primary_lightgreen`, `winter_white`, `summer_yellow`).

## Layout

- **Content width:** 1180px (130px side margins at 1440). Below that, 50px side margins.
- **Image bands:** full width, 1024px tall (993px on mobile). Hero, massage room and lounge.
- **Card rows:** cards 420 x 740 (mobile 340 x 748), 40px gap (mobile 30px), 30px padding. Each row overlaps the band above by 60px and scrolls sideways; the third card bleeds past the right edge as in the design.
- **Card colours by season:** green intro card, `winter-white` (Fuyu / winter), `summer-yellow` (Natsu / summer), light greens for offers.
- **Card bottom stack:** description, 40px, divider, 40px, price block, 80px, fine print, 30px padding.
- **Footer:** green, three 380px columns with 20px gap (socials + contact, message form, map placeholder), logo row 50px below.

## Text boxes

Figma trims text to cap height. `.trim` uses `text-box: trim-both cap alphabetic` so CSS spacing values are the Figma ones. Browsers without `text-box` support show a few extra pixels of line spacing.

## Assets

All in `images/`, exported from Figma: `hero-bg.jpg`, `massage-room.jpg`, `lounge.jpg`, logo icon and wordmark (white header, light green footer), social icons, arrow lines, dividers.
