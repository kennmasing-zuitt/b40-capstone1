---
name: AltMobility Philippines
colors:
  base: '#30506e'
  white: '#ffffff'
  dark-gray: '#5c6b73'
  text-gray: '#666666'
  charcoal: '#43454a'
  rights-blue: '#72a1b4'
  sidebar-accent: '#47748b'
  sidebar-hover: '#7386d5'
  body-olive: '#5f7053'
  button-border: 'rgba(148, 148, 148, 0.5)'
  sidebar-panel: 'rgba(0, 0, 0, 0.75)'
  overlay: 'rgba(0, 0, 0, 0.7)'
  line-pnr: orange
  line-lrt1: '#fff23b'
  line-lrt2: '#924ac2'
  line-mrt3: '#3f94fc'
  line-4: '#fa66fa'
  line-5: '#7acc54'
  line-6: '#eb9d31'
  line-7: '#963d27'
  line-8: '#754e1b'
  line-9: '#db0000'
  line-pnr-north: '#126e3d'
  line-pnr-south: '#0c5b82'
typography:
  display-hero:
    fontFamily: Oswald
    fontSize: 112px
    fontWeight: '500'
    lineHeight: 134.4px
  display-hero-mobile:
    fontFamily: Oswald
    fontSize: 40px
    fontWeight: '500'
    lineHeight: 48px
  hero-sub:
    fontFamily: Saira Extra Condensed
    fontSize: 48px
    fontWeight: '400'
    lineHeight: 72px
  hero-sub-mobile:
    fontFamily: Saira Extra Condensed
    fontSize: 19.2px
    fontWeight: '400'
    lineHeight: 28.8px
  section-title:
    fontFamily: Oswald
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 60px
  section-title-mobile:
    fontFamily: Oswald
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 36px
  headline-md:
    fontFamily: Oswald
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 38.4px
  card-title:
    fontFamily: Oswald
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 50px
  card-title-sm:
    fontFamily: Oswald
    fontSize: 20px
    fontWeight: '700'
    lineHeight: 30px
  quote:
    fontFamily: Arial
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
  subhead-condensed:
    fontFamily: Saira Extra Condensed
    fontSize: 24px
    fontWeight: '400'
    lineHeight: 36px
  list-heading:
    fontFamily: Arial Narrow
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 33.6px
  body-md:
    fontFamily: Arial
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Arial
    fontSize: 14.4px
    fontWeight: '400'
    lineHeight: 21.6px
  nav-link:
    fontFamily: Calibri
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
rounded:
  DEFAULT: 0.375rem
  button: 5px
  full: 50rem
spacing:
  section-min-height: 100vh
  card-gap: 1rem
  nav-height: 60px
  nav-height-desktop: 94px
  breakpoint-photo: 576px
  breakpoint-tablet: 768px
  breakpoint-desktop: 992px
  breakpoint-wide: 1400px
---

## Brand & Style

AltMobility Philippines is a one-page advocacy site for commuters' rights in Metro Manila. It speaks to daily commuters, voters ahead of Halalan 2022 and anyone who walks, bikes or takes the train. The tone is civic and urgent but hopeful: big campaign headlines (`#COMMUTERSNAMAN`), plain facts about rail lines and street design, and clear calls to sign up and vote.

The look is a **campaign poster on a calm blue base**:
- **Full-screen photo sections** (EDSA traffic, commuters, the contact backdrop) set the mood behind white display type.
- **White content sections** carry the facts: the Bill of Rights cards, the rail-line cards and the NACTO street comparison.
- **Condensed type everywhere**: Oswald for headlines, Saira Extra Condensed for spaced-out subheads (`J O I N   T H E   C O N V E R S A T I O N`).

## Colors

- **Base Blue (`#30506e`):** Page background, the navbar, the footer, and the mobile menu's header and close button. The single brand colour; every dark band on the page uses it.
- **White (`#ffffff`):** Display type over photos, text on blue, and the background of the fact sections.
- **Rights Blue (`#72a1b4`):** Fill of the five Commuter's Bill of Rights cards, with white titles and text. White on it is only 2.81:1, below WCAG AA for both normal (4.5:1) and large text (3:1), so the card titles fail too. Kept as is to preserve the look; darken it before relying on it for readable text.
- **Text Gray (`#666666`) and Charcoal (`#43454a`):** Headings inside white sections. Gray: section titles, rail line-group headings, and the NACTO title and captions below desktop. Charcoal: rail-line card titles, and the NACTO title and captions on desktop.
- **Body Olive (`#5f7053`):** Description paragraphs in the white sections.
- **Dark Gray (`#5c6b73`):** The "Know more" buttons. Every other link is white (mobile menu links turn Sidebar Hover on hover). Links have no underline, except on hover for the navbar, article and footer call-to-action links.
- **Sidebar Accent (`#47748b`) and Sidebar Hover (`#7386d5`):** The rule under the mobile menu links, and the hover colour of its links and close button.
- **Rail line colours (`--line-*`):** Each line card has a 5px left marker in that line's colour, for example LRT-1 yellow `#fff23b`, LRT-2 purple `#924ac2` and MRT-3 blue `#3f94fc`. They identify lines only; don't reuse them for UI.
- **Button Border (`rgba(148, 148, 148, 0.5)`):** Outline of the "Know more" buttons.
- **Sidebar Panel (`rgba(0, 0, 0, 0.75)`):** Background of the mobile menu.
- **Overlay (`rgba(0, 0, 0, 0.7)`):** Bootstrap's backdrop behind the open mobile menu (`--bs-backdrop-bg: var(--color-overlay)`).

Every site colour above is a custom property in the `:root` block of `index.css` (`--color-*` and `--line-*`). Use the variable, not the literal, when adding rules. Shadows and a few one-off greys stay literal.

## Typography

- **Display & Section Titles (Oswald):** Sizes scale with the screen width (`clamp()`). The hero headline goes from 40px on phones to 62px at 800px, and is 112px on desktop (from 992px). Section titles go from 24px (390px) to 33px at 800px and 40px bold from about 1150px. Card titles: Bill of Rights 19.2px below desktop and 24px on desktop; rail lines 16px and 24px; NACTO captions 14.4px and 20px. The hero and Bill of Rights titles wrap long words rather than overflow if the web font hasn't loaded. Mostly uppercase in the markup.
- **Condensed Subheads (Saira Extra Condensed):** Letter-spaced hero subtitles, the `2 0 2 2` Halalan year and contact subheads. The spacing is typed into the text, so keep it when editing copy.
- **Body (Arial):** Descriptions, card text, the "Know more" buttons and the featured quote (40px bold on desktop, 32px below).
- **List Headings (Arial Narrow):** "EXISTING LINES"-style headings in the rail section.
- **Navigation (Calibri):** Desktop navbar links.
- **System font (Bootstrap default):** Forms, the pill buttons, the Halalan call to action, the article labels, the copyright line and, below desktop, the legal links (Oswald on desktop).

The font stacks are `--font-display`, `--font-condensed`, `--font-body` and `--font-narrow` in `:root`. Fonts load from one Google Fonts stylesheet (`Oswald` and `Saira Extra Condensed`, `display=swap`), which then fetches the font files. Arial, Arial Narrow and Calibri are system fonts.

## Layout & Spacing

- **One page for every screen:** each section exists once in `index.html`, inside `<main>` between the navbar and the footer, and adapts with Bootstrap 5 classes (`d-none d-lg-block`, `col-5 col-lg`) plus mobile-first media queries in `index.css`.
- **Section heights follow content:** desktop sections have `min-height: 100vh` (contact `80vh`) and grow when their content needs more room. No section has a fixed height; only images, controls and the rail line markers do (for example the NACTO GIFs are `35vh` tall below desktop).
- **Breakpoints:** Bootstrap's, mobile first: `576px` (desktop hero photo), `768px` (Halalan panel up to 540px wide), `992px` desktop (full navbar, side-by-side layouts), `1400px` wide (roomier navbar).
- **Sticky navbar:** anchor links scroll the section to just under the navbar (`scroll-padding-top: var(--nav-height)`, 60px below desktop and 94px on desktop, where the logo is a fixed 64px tall).
- **Grid:** the Bill of Rights and rail cards sit in Bootstrap rows (`col-5 col-lg`): one row on desktop, two per row below, with a `1rem` gap (`0.5rem` margin on each card). The NACTO GIFs are four columns on desktop and two below (`col-6 col-lg-3`).
- **Hidden below desktop:** the Bill of Rights intro and card descriptions, the NACTO description and the rail network map.
- **Images below the hero load lazily** (`loading="lazy"`) and carry their real `width`/`height`, with `height: auto` in the CSS, so nothing moves while they load and anchor links land in the right place. Phones never download the hidden rail map.

## Elevation & Depth

The site is flat. Depth comes from photography, not shadows: on desktop the contact photo stays fixed while the page scrolls over it (`background-attachment: fixed`). The only shadows are the navbar's `1px 1px 3px rgba(0, 0, 0, 0.1)` and the mobile menu's drop shadow. The menu slides in over a 70% black backdrop.

## Shapes

- **Cards:** Bootstrap 5's default `0.375rem` corners.
- **Buttons:** "Know more" buttons use `5px` corners with a `1.5px solid rgba(148, 148, 148, 0.5)` border on a transparent background.
- **Pills:** the search field and the outline buttons (Submit, Send Message, Contribute) are fully rounded with a light outline.

## Components

### Navbar
- Sticky Base Blue bar. Desktop: the AltMobility logo on the left, Calibri links to each section in the middle and a pill search field on the right. Below desktop: a menu button on the left and the logo centred. The search field is a placeholder: searching reloads the page.

### Mobile Menu
- Bootstrap's offcanvas panel (`#sidebar`, 250px) slides in from the left: a Base Blue header with the logo and close button, the section links and a search field on a 75% black panel. Tapping a link closes the menu, adds the section to the URL and Back history (unless it is already there), moves keyboard focus to the section and scrolls it under the navbar. Taps are ignored while the panel is still sliding, and the menu closes by itself if the window is widened to desktop. The close button, the backdrop and Esc also close it. The panel scrolls when it is taller than the screen. No jQuery.

### Hero
- Full-screen photo with the `#COMMUTERSNAMAN` headline in Oswald and a spaced-out Saira subtitle.

### Bill of Rights Cards
- Five Rights Blue cards (Safe, Reliable, Accessible, Comfortable, Sustainable), each with an icon, an Oswald title and white body text (desktop only). They flip in on scroll (AOS `flip-left`).

### Rail Line Cards
- White cards with a coloured line marker (`--line-*`) before the line name and the line's logo below. Existing and future lines are grouped, next to the rail network map on desktop.

### Halalan Panel
- Bottom right of the Join Us photo, under the featured-article quote: a fingerprint icon, `H A L A L A N` in Oswald, `2 0 2 2` in Saira and a "Magpa-rehistro, bumoto!" call to action.

### NACTO Comparison
- Four animated GIFs (car lane, bike lane, sidewalk, transitway) with Oswald captions and people-per-hour figures; the title and description sit to the right on desktop and above the GIFs below.

### Contact
- Newsletter signup, social icons (Font Awesome), contact details and a demo CAPTCHA over a photo, in two columns on desktop and one below. The forms are demo content: they have no backend, so submitting reloads the page without sending anything.

### Footer
- Base Blue band with the logo, the `J O I N   T H E   C O N V E R S A T I O N` link, a Contribute button (a placeholder with no action yet), social icons (below desktop), placeholder legal links (`#`) and the copyright line.
