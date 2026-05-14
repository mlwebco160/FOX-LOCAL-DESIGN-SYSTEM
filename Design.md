## Purpose
This file defines the visual style, design tokens, and component guidelines for the FOX LOCAL mobile app. AI coding tools should follow this file when generating or modifying UI.

## Product Style

Tone & Personality
FOX LOCAL should feel like a local news mobile app (think Apple News) not a lifestyle app. The design communicates:

Authority — bold type, high contrast, minimal decoration
Density — high information-per-screen, respects the user's time
Trust — consistent branding, clean hierarchy, no clutter
Urgency — red accents labels for live and breaking content

Avoid anything that feels soft, playful, or decorative. Every design decision should ask: does this help a user get to the news faster?


## Overview

FOX LOCAL has a bold, authoritative visual identity designed for trust, urgency, and fast information consumption. The aesthetic draws from broadcast news traditions while feeling native to modern mobile — dark, dense, and confident without being overwhelming.

---

## Color Palette

| Role | Value | Usage |
|---|---|---|
| Primary Background | `#042152` (deep navy) | Screen backgrounds, card fills |
| Secondary Background | `#19305F` (mid navy) | Section containers, trending cards |
| Surface / Card | `#19305F` (lighter navy) | Elevated cards, video thumbnails |
| Accent Color Red | `#D20F26` (FOX red) | "Watch Live" CTA button, live badges |
| Accent Color Blue | `#4378D4` | Buttons, badges, bullet points |
| Text — Primary | `#FFFFFF` | Headlines, story titles, category tags |
| Text — Secondary | `#8A9BB8` (muted blue-gray) | Timestamps, bylines, metadata |
| Text — Tertiary | `#C5CED9` | Supporting body copy |
| Live Badge | `#E8192C` with white label | LIVE indicator on streams |

The palette is intentionally limited: deep navy owns the canvas, white text for headers and headlines, while FOX red or blue accent colors punctuates only the most important interactive or live elements. No gradients, no decorative colors — urgency through restraint.

---

## Typography

- **Headlines / Story Titles**: Bold weight, white, large — typically 18–24pt. Tight line-height to pack impact. No truncation on hero stories; full headline always visible.
- **Section Headers** (e.g., "Top Stories from FOX 11", "Trending", "Crime & Public Safety"): Bold white, 20–22pt. Left-aligned. Some sections pair a header with a small icon or `+` action button.
- **Article Body Copy**: Regular weight, ~15–16pt, muted blue-gray (`#8A9BB8`) for secondary text, white for in-article body text. Comfortable line-height for reading.
- **Metadata / Timestamps**: Small, ~12–13pt, muted blue-gray. Always below or beside the headline.
- **"The Brief" Bullets**: Bold white, large (~18pt), generous line-height. Bullet points use FOX blue dots. Designed for skimmability.

**Font character**: Rubik Font Family - System-weight sans-serif, no decorative or serif fonts. The typography is utilitarian and news-grade — prioritize legibility and density over style.

---

## Layout & Spacing

- **Full-bleed dark background** — no white space used decoratively; the dark navy IS the canvas.
- **Card-based content system**: Stories live in rounded-corner cards (`border-radius: ~12px`) that sit slightly elevated against the background navy.
- **Hero image + headline pattern**: Lead stories use a full-width image above a large bold headline. Below-the-fold stories switch to a horizontal thumbnail-left, headline-right layout.
- **Horizontal scroll carousels**: Used for "Latest Videos" and "Crime & Public Safety" category sections — cards peek at the right edge to signal scrollability.
- **Trending list**: Numbered items (1, 2, 3…) in circular badges, with title text and an optional video play icon. Dividers between items are subtle, hairline-weight.
- **Section spacing**: Generous vertical padding between sections (~24–32pt). Section headers always have breathing room above them.
- **Content density**: High — multiple story types (hero, grid, list, carousel, show posters) on a single scroll. No wasted whitespace between content sections.

---

## Iconography & Interactive Elements

- **"Watch Live" Button**: rectangle-shaped, with radius of 4px, solid FOX red (`#D20F26`), bold white label. Always top-right in the navigation bar. This is the primary CTA and should always be immediately visible.
- **LIVE badge**: Small red rectangle-shaped with white "LIVE" text (radius of 2px). Appears on the active livestream card.
- **Play button overlay**: Semi-transparent circular play icon centered over video thumbnails. Consistent across all video types.
- **Expand/fullscreen icon**: Appears bottom-right of the livestream card. Minimal, white, 2-color icon.
- **Search icon**: Top-left nav, white outline style.
- **Weather icon**: Top-left nav beside search, matches system-style cloud icon, white.
- **Video duration badge**: Small dark-background pill (e.g., `3:35`, `44:35`) bottom-right of video thumbnails.
- **"+" icon**: Appears beside certain section headers (e.g., "National News +") to indicate a follow/add action.

---

## Navigation & Header

- **Top bar**: Minimal. FOX LOCAL logo (https://github.com/mlwebco160/FOX-LOCAL-DESIGN-SYSTEM/blob/10984b0131629de20fc37a0b7cff299f1768d750/images/FOX-LOCAL-Logo-Horizontal.png) at the top, centered. Search + Weather icons left. "Watch Live" button right. No tab bar visible in these screens — content is scroll-driven.
- **Article detail nav**: Adds a horizontal scrollable topic tag strip below the header (e.g., "Heat Dome 2024 · Heat Dome set to sizzle · Extre…"), using a red dot live indicator for active topics.
- The header background bleeds into the page — no border or shadow separator.

---

## Article / Story Detail View

- Category label + timestamp at top (e.g., "News · 5 min ago"), muted.
- Large bold headline, followed by a short italic-style dek/subhead.
- Byline in muted blue-gray.
- Full-width embedded video or image.
- **"The Brief"** section: Bulleted key facts in bold white — designed for skim-reading before the full article.
- **"The Source"** callout: Slightly elevated card with darker background, bold label, plain body text. Used to attribute data.
- **"What we know"** section: Bold inline label followed by full article body text in white, regular weight.

---

## Motion & Interactions

- Transitions should be **fast and functional** — this is a news app, not entertainment. Aim for 200–300ms standard transitions.
- No decorative animations; motion is reserved for page transitions and video play states.
- Scroll behavior is standard momentum scroll — no snap or parallax on the feed.
- Carousel swipes should feel native-responsive with slight deceleration.

