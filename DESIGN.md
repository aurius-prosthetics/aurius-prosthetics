---
name: Aurius Prosthetics
description: Open-source 3D-printed prosthetic ears, presented as a quiet monochrome clinical-editorial site.
colors:
  ink-black: "#111111"
  charcoal: "#1C1C1C"
  true-black: "#000000"
  paper: "#FAFAFA"
  white: "#FFFFFF"
  hairline-grey: "#E8E8E8"
  label-grey: "#6B6B6B"
  body-grey: "#555555"
typography:
  display:
    fontFamily: "Raleway, sans-serif"
    fontSize: "clamp(2.4rem, 5.5vw, 4.2rem)"
    fontWeight: 300
    lineHeight: 1.15
    letterSpacing: "0.04em"
  headline:
    fontFamily: "Raleway, sans-serif"
    fontSize: "clamp(1.8rem, 3.5vw, 2.8rem)"
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: "0.02em"
  title:
    fontFamily: "Raleway, sans-serif"
    fontSize: "1.1rem"
    fontWeight: 600
    letterSpacing: "0.06em"
  body:
    fontFamily: "Raleway, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 400
    lineHeight: 1.8
    letterSpacing: "0.01em"
  label:
    fontFamily: "Raleway, sans-serif"
    fontSize: "0.68rem"
    fontWeight: 600
    letterSpacing: "0.2em"
rounded:
  none: "0px"
  dot: "50%"
spacing:
  section-y: "96px"
  section-x: "48px"
  section-x-mobile: "20px"
  container: "1080px"
components:
  button-light:
    backgroundColor: "{colors.white}"
    textColor: "{colors.charcoal}"
    rounded: "{rounded.none}"
    padding: "14.4px 35.2px"
  button-dark:
    backgroundColor: "{colors.charcoal}"
    textColor: "{colors.white}"
    rounded: "{rounded.none}"
    padding: "14.4px 35.2px"
  button-dark-hover:
    backgroundColor: "{colors.true-black}"
  nav:
    backgroundColor: "{colors.ink-black}"
    textColor: "{colors.white}"
    height: "72px"
---

# Design System: Aurius Prosthetics

## Overview

**Creative North Star: "The Clinical Monograph"**

A monochrome, almost entirely typographic system that lets photography of ears, scans and printed prosthetics carry all the colour and emotion. It reads like a printed medical monograph: wide letter-spaced capitals for labels, light-weight Raleway for large statements, hairline rules instead of boxes, and generous vertical air. The tone is calm and credible, because the audience is people with microtia, their families, and clinicians.

Density is low and sections alternate between near-black and paper white, so each page reads as a sequence of single ideas. Nothing is decorative; structure comes from rules, spacing and weight contrast (300 against 600/700) within one typeface.

**Key Characteristics:**
- One typeface (Raleway); hierarchy comes from weight, case and tracking, never from a second family.
- Strictly neutral palette; no accent colour. Imagery supplies all hue.
- Square corners, hairline dividers, zero shadows.
- Dark hero and process bands alternating with paper-white reading sections.
- Quiet motion: fade pages and scroll reveals only.

## Colors

A true greyscale: two near-blacks, two whites, and grey steps for hierarchy. Accent is intentionally absent.

### Neutral
- **Ink Black** (#111111): page canvas for hero, process, tagline, price and contact hero bands; nav at 96% opacity.
- **Charcoal** (#1C1C1C): primary text on light, dark-button fill, ticker banner.
- **True Black** (#000000): footer and dark-button hover.
- **Paper** (#FAFAFA): default page background and the second half of the mission strip.
- **White** (#FFFFFF): reading sections, light button fill, text on dark.
- **Hairline Grey** (#E8E8E8): 1px dividers and role-card gutters.
- **Label Grey** (#6B6B6B): eyebrows, spec labels, captions on light grounds (4.9:1 on white).
- **Body Grey** (#555555): long-form paragraphs on light grounds.

### Named Rules
**The No-Accent Rule.** Never introduce a brand colour. Emphasis comes from weight, case and inversion between dark and light bands.

**The Readable Grey Rule.** Text on dark never falls below 55% white; small text on light never lighter than #6B6B6B. Decorative low-opacity text is not allowed to carry information.

## Typography

**Display / Body / Label Font:** Raleway (Google Fonts, 300–700 plus italic 400/500), sans-serif fallback.

**Character:** Geometric and airy at light weights, firm at 600–700. Lining numerals are forced (`font-variant-numeric: lining-nums`) because Raleway defaults to old-style figures, which misread prices and specs.

### Hierarchy
- **Display** (300, clamp 2.4–4.2rem, 1.15): hero title; the key phrase switches to 600 via `<strong>`.
- **Headline** (300, clamp 1.8–2.8rem, 1.2): section titles; page-hero titles use 300 with a 700 emphasis word.
- **Title** (600, 1.1rem, tracking 0.06em): process step titles, role titles, collaborator names.
- **Body** (400, 0.9375rem, 1.8, tracking 0.01em): paragraphs, capped at 640px (about 65ch).
- **Label** (600, 0.68–0.75rem, tracking 0.15–0.22em, uppercase): eyebrows, nav, buttons, spec keys, step numbers.

### Named Rules
**The Weight-Contrast Rule.** Headlines pair a 300 phrase with one 600/700 phrase. Never bold a whole heading.

**The Wide-Caps Rule.** Uppercase is always tracked 0.12em or more; body text is never uppercase.

## Layout

Single 1080px centred container inside full-bleed colour bands. Section padding is 96px vertical, 48px horizontal (20px horizontal and 56px vertical at ≤900px). Two-column grids (3fr/2fr on About, 1fr/1fr on Gallery, Contact and Mission) collapse to one column at 900px; the three-up process and roles grids stack. The site is a single document with four in-page views (Home, About, Gallery, Contact) that fade between each other; each ends in the same footer.

The fixed nav is 72px tall plus the iOS safe-area inset; page content is offset by the same amount. Below 900px the links collapse into a full-screen overlay menu behind a hamburger.

## Elevation & Depth

Flat. There are no shadows. Depth is conveyed by alternating dark and light bands, 1px hairlines, and photography dimmed under dark gradient overlays (hero image at 38% opacity, About at 25%, Gallery video at 55%). The only translucency is the nav's 8px backdrop blur.

### Named Rules
**The Flat-By-Default Rule.** Nothing lifts. State changes are colour or border changes, never shadow.

## Shapes

Square. Buttons, cards, images and rules are all rectangular with 0 radius; the single circle is the 6px pulsing dot in the ticker. Borders are 1px hairlines, with a 2px charcoal rule used once per sidebar to anchor a column. The pull-quote uses a 2px left rule.

## Components

### Buttons
- **Shape:** rectangular, 0 radius, label-style type (600, 0.72rem, 0.16em tracking, uppercase).
- **Light (on dark):** white fill, charcoal text; hover softens to #E8E8E8.
- **Outline light:** transparent with 45%-white border; hover adds 10% white wash and a full white border.
- **Dark (on light):** charcoal fill; hover to true black. **Outline dark** fills charcoal on hover.
- **Focus:** 2px outline, 4px offset (white on dark grounds, charcoal on light).

### Navigation
Fixed ink-black bar. Wordmark in 600 caps with 0.18em tracking (the logo; never altered). Links in 0.75rem caps, 72% white, with a 1px underline for hover and active. Mobile: 44px hamburger, full-screen overlay with 1.5rem light-weight links separated by hairlines.

### Process Item
Numbered step label, 280px-tall image (220px on mobile), title, short description, divided from neighbours by a hairline.

### Role Card / Collaborator Row
Role cards sit in a 1px-gap grid on hairline grey, white fill, 40px/32px padding. Collaborator rows are name (600) plus role line separated by hairlines.

### Spec Table
Two-column, label in tracked caps grey, value in regular charcoal, 1px row rules.

### Stat Block
Struck-through old price in muted grey, arrow, then the new figure at 700 up to 7rem; a caption in tracked caps.

## Do's and Don'ts

### Do:
- **Do** keep every surface greyscale; let photography be the colour.
- **Do** build hierarchy with 300 versus 600/700 weight, case, and tracking.
- **Do** separate content with 1px hairlines and alternating dark/light bands.
- **Do** respect `prefers-reduced-motion`: reveals and the ticker pulse switch off.
- **Do** keep focus outlines visible on every interactive element.

### Don't:
- **Don't** add shadows, rounded corners, gradients on text, or an accent colour.
- **Don't** introduce a second typeface.
- **Don't** set text on dark below 55% white or small text on light lighter than #6B6B6B.
- **Don't** alter the wordmark's weight, tracking or case.
