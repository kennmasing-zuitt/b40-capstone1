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
  line-subway: gray
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
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 42px
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
    lineHeight: 24px
  quote:
    fontFamily: Arial
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
  subhead-condensed:
    fontFamily: Saira Extra Condensed
    fontSize: 24px
    fontWeight: '400'
    lineHeight: 28.8px
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
  DEFAULT: 0.25rem
  button: 5px
  full: 50rem
spacing:
  section-height: 100vh
  card-gap: 1rem
  breakpoint-small-phone: 411px
  breakpoint-phone: 576px
  breakpoint-small-tablet: 767px
  breakpoint-tablet: 991px
  breakpoint-desktop: 992px
---

## Brand & Style

AltMobility Philippines is a one-page advocacy site for commuters' rights in Metro Manila. It speaks to daily commuters, voters ahead of Halalan 2022 and anyone who walks, bikes or takes the train. The tone is civic and urgent but hopeful: big campaign headlines (`#COMMUTERSNAMAN`), plain facts about rail lines and street design, and clear calls to sign up and vote.

The look is a **campaign poster on a calm blue base**:
- **Full-screen photo sections** (EDSA traffic, commuters, the contact backdrop) set the mood behind white display type.
- **White content sections** carry the facts: the Bill of Rights cards, the rail-line cards and the NACTO street comparison.
- **Condensed type everywhere**: Oswald for headlines, Saira Extra Condensed for spaced-out subheads (`J O I N   T H E   C O N V E R S A T I O N`).

## Colors

- **Base Blue (`#30506e`):** Page background, desktop navbar, footers, and the mobile sidebar's header and close button. The single brand colour; every dark band on the page uses it.
- **White (`#ffffff`):** Display type over photos, text on blue, and the background of the fact sections.
- **Rights Blue (`#72a1b4`):** Fill of the five Commuter's Bill of Rights cards, with white text. It only reaches 2.81:1 contrast with white, which is below WCAG AA; fix it before relying on it for body text.
- **Text Gray (`#666666`) and Charcoal (`#43454a`):** Headings inside white sections. Gray: section titles, rail-network headings and the mobile NACTO captions. Charcoal: rail-line card titles, the desktop NACTO title and its captions.
- **Body Olive (`#5f7053`):** Description paragraphs in the white sections.
- **Dark Gray (`#5c6b73`):** The "Know more" button links. Other links keep Bootstrap's default blue (`#007bff`).
- **Sidebar Accent (`#47748b`) and Sidebar Hover (`#7386d5`):** Mobile sidebar list rules and the close-button hover.
- **Rail line colours (`--line-*`):** Each line card has a 5px left marker in that line's colour, for example LRT-1 yellow `#fff23b`, LRT-2 purple `#924ac2` and MRT-3 blue `#3f94fc`. They identify lines only; don't reuse them for UI.
- **Button Border (`rgba(148, 148, 148, 0.5)`):** Outline of the "Know more" buttons.
- **Sidebar Panel (`rgba(0, 0, 0, 0.75)`):** Background of the mobile sidebar's link list.
- **Overlay (`rgba(0, 0, 0, 0.7)`):** Dims the page while the mobile sidebar is open.

Every colour above is a custom property in the `:root` block of `index.css` (`--color-*` and `--line-*`). Use the variable, not the literal, when adding rules. Shadows and a few one-off greys stay literal.

## Typography

- **Display & Section Titles (Oswald):** The hero headline is 112px on desktop, 80px on tablets (768–991px), 48px at 412–576px and 40px at 411px and below. Section titles are 40px bold on desktop. On phones the Bill of Rights title is 32px (412–576px) or 28px (411px and below), the NACTO title 32px or 24px, and the rail title 24px. Mostly uppercase in the markup.
- **Condensed Subheads (Saira Extra Condensed):** Letter-spaced hero subtitles, the `2 0 2 2` Halalan year and contact subheads. The spacing is typed into the text, so keep it when editing copy.
- **Body (Arial):** Descriptions, card text, the "Know more" buttons and the featured quote (40px bold on desktop).
- **List Headings (Arial Narrow):** "EXISTING LINES"-style headings in the rail section.
- **Navigation (Calibri):** Desktop navbar links.
- **System font (Bootstrap default):** Forms, the pill buttons, the Halalan call to action and small print.

Fonts load from one Google Fonts stylesheet (`Oswald` and `Saira Extra Condensed`, `display=swap`), which then fetches the font files. Arial, Arial Narrow and Calibri are system fonts.

## Layout & Spacing

- **Fixed section heights:** on desktop most sections are `100vh`, contact is `80vh` and the footer `20vh`. Below desktop some sections grow to fixed heights instead of sizing to content: the rail section is `200vh` at 577–991px and `170vh` on phones, and contact is `170vh`–`180vh` on phones.
- **Bootstrap 4 grid:** the Bill of Rights and rail cards are Bootstrap `card` elements in rows (`col-5 col-lg`), wrapping two per row below desktop, with a `1rem` gap (`mx-2 my-2` on each card).
- **Breakpoints:** `index.css` uses its own closed ranges: ≤411px, 412–576px, 577–767px, 768–991px and ≥992px. They don't match Bootstrap's breakpoints.
- **Copies per screen size:** `index.html` has a desktop navbar plus a mobile sidebar, three versions of the hero text, desktop and mobile versions of the Join Us cards (inside one section), two NACTO sections and two footers. CSS hides the copies that don't fit the screen. Edit every copy until they are merged.
- **Hidden below desktop:** the Bill of Rights card descriptions and the rail network map.

## Elevation & Depth

The site is flat. Depth comes from photography and the parallax background in the contact section, not from shadows. The only shadows are the navbar's `1px 1px 3px rgba(0, 0, 0, 0.1)` and the mobile sidebar's drop shadow. The sidebar slides in over a 70% black overlay.

## Shapes

- **Cards:** Bootstrap's default `0.25rem` corners.
- **Buttons:** "Know more" buttons use `5px` corners with a `1.5px solid rgba(148, 148, 148, 0.5)` border on a transparent background.
- **Pills:** the search field and the newsletter Submit button are fully rounded (Bootstrap `rounded-pill`) with a light outline.

## Components

### Desktop Navbar
- Sticky Base Blue bar: the AltMobility logo on the left, Calibri links to each section in the middle column, and a pill search field on the right.

### Mobile Sidebar
- A hamburger button opens a sidebar from the left: a Base Blue header with the logo and close button, and the section links on a 75% black panel. Tapping a link or the dark overlay closes it.

### Hero
- Full-screen photo with the `#COMMUTERSNAMAN` headline in Oswald and a spaced-out Saira subtitle.

### Bill of Rights Cards
- Five Rights Blue cards (Safe, Reliable, Accessible, Comfortable, Sustainable), each with an icon, an Oswald title and white body text (desktop only). They flip in on scroll (AOS `flip-left`).

### Rail Line Cards
- White cards with a coloured line marker (`--line-*`) before the line name and the line's logo below. Existing and future lines are grouped, next to the rail network map on desktop.

### Halalan Panel
- A card over the Join Us photo: a fingerprint icon, `H A L A L A N` in Oswald, `2 0 2 2` in Saira and a "Magpa-rehistro, bumoto!" call to action.

### NACTO Comparison
- Four animated GIFs (car lane, bike lane, sidewalk, transit) with Oswald captions and people-per-hour figures.

### Contact
- Newsletter signup, social icons (Font Awesome), contact details and a demo CAPTCHA over a parallax photo. The forms are demo content: they have no backend, so submitting reloads the page without sending anything.

### Footer
- Base Blue band with the logo, a Contribute button, placeholder legal links (`#`) and the copyright line.
