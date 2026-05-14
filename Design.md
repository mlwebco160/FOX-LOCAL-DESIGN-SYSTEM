## Purpose
This file defines the visual style, design tokens, and component guidelines for the FOX LOCAL mobile app. AI coding tools should follow this file when generating or modifying UI.

# FOX LOCAL — Design System

## Key Characteristics

- Deep navy broadcast-inspired dark theme (`#042152`–`#19305F`) optimized for live news consumption
- FOX Red (`#D20F26`) reserved for urgency, LIVE states, breaking news, and primary CTAs
- Dense, information-forward layout philosophy — maximize useful content per screen
- Strong editorial hierarchy using bold headlines and restrained supporting metadata
- Rounded card system (`8px–12px`) that modernizes broadcast aesthetics without becoming soft
- Mobile-first layouts optimized for fast scanning and continuous feed consumption
- Livestream-first architecture — video is a primary surface, not secondary content
- Minimal decorative motion; transitions are fast, functional, and newsroom-grade
- High-contrast typography optimized for readability across mobile and connected TV
- Modular feed composition using hero stories, trending stacks, live rails, weather modules, and video carousels

---

# 1. Visual Theme & Atmosphere

FOX LOCAL is a dark, fast-moving streaming news platform designed for immediacy, trust, and continuous information consumption. The interface combines the authority of broadcast television with the fluidity and responsiveness of a modern mobile product. The design philosophy is “information-first urgency” — the interface exists to surface local news, weather, and live coverage with maximum clarity and minimum friction.

The visual foundation is built on deep navy and near-black surfaces (`#042152`, `#19305F`) that create a stable newsroom-grade environment where headlines, live video, and breaking alerts dominate attention. Unlike entertainment platforms that prioritize atmosphere or immersion, FOX LOCAL prioritizes scanning efficiency, editorial hierarchy, and content throughput.

White typography provides strong contrast against the dark foundation, while FOX Red (`#D20F26`) acts as a restrained urgency signal reserved for live programming, breaking news, severe weather, and primary calls-to-action. Accent Blue (`#4378D4`) supports secondary actions, bullet indicators, and informational modules without competing against the urgency system.

Typography is bold, dense, and utilitarian. Headlines carry most of the visual weight, designed for immediate comprehension and authority. Supporting metadata recedes into muted blue-gray tones to preserve hierarchy while maintaining context. The system favors compact spacing, strong alignment, and minimal stylistic flourish.

The geometry system is intentionally restrained. Cards use subtle radii (`8px–12px`) to modernize the broadcast aesthetic while maintaining seriousness and urgency. Unlike entertainment or social apps, FOX LOCAL avoids oversized pills, playful softness, floating glass effects, or exaggerated animation.

Motion is operational rather than expressive. Transitions should feel immediate and responsive (`200ms–300ms`) with motion used only to support navigation, playback, feed updates, and hierarchy changes. The interface should feel alive and continuously updating, but never cinematic or decorative.

Overall, FOX LOCAL should feel like a premium real-time local news command center: authoritative, trustworthy, dense, fast-moving, and optimized for live information delivery across mobile and connected TV platforms.

---

# 2. Color Palette & Roles

## Primary Brand

- **Deep Navy** (`#042152`) — Primary application background
- **Mid Navy** (`#19305F`) — Elevated surfaces, containers, modules
- **FOX Red** (`#D20F26`) — LIVE states, breaking news, primary CTA
- **FOX Blue** (`#4378D4`) — Secondary actions, informational accents

## Text

- **Primary White** (`#FFFFFF`) — Headlines, titles, primary labels
- **Muted Blue Gray** (`#8A9BB8`) — Metadata, timestamps, bylines
- **Secondary Light Gray** (`#C5CED9`) — Supporting text, descriptions
- **Muted Dark Text** (`#5F6B82`) — Disabled states, low-priority metadata

## Semantic

- **Breaking Red** (`#E8192C`) — Severe urgency, live indicators
- **Weather Yellow** (`#FFC857`) — Weather alerts and advisories
- **Success Green** (`#3FB950`) — Positive system confirmations
- **Warning Orange** (`#FF9F1C`) — Moderate alerts or advisories

## Surface & Border

- **Primary Surface** (`#19305F`) — Main card surfaces
- **Secondary Surface** (`#223B72`) — Alternate elevated surfaces
- **Divider** (`rgba(255,255,255,0.08)`) — Hairline separators
- **Border Subtle** (`rgba(255,255,255,0.12)`) — Low-contrast borders
- **Overlay Surface** (`rgba(4,33,82,0.92)`) — Floating overlays and menus

## Shadows

- **Card Shadow** (`rgba(0,0,0,0.24) 0px 4px 12px`) — Elevated cards
- **Modal Shadow** (`rgba(0,0,0,0.45) 0px 12px 32px`) — Dialogs and overlays
- **Video Overlay** (`linear-gradient(180deg, rgba(0,0,0,0) 0%, rgba(0,0,0,0.72) 100%)`) — Headline readability over media

---

# 3. Typography Rules

## Font Families

- **Primary UI Font**: `Rubik`
- **Fallback Stack**: `Inter, SF Pro Display, Roboto, Helvetica Neue, Arial, sans-serif`

## Hierarchy

| Role | Size | Weight | Line Height | Notes |
|---|---|---|---|---|
| Hero Headline | 28px–34px | 700 | Tight | Breaking or lead story |
| Story Headline | 18px–24px | 700 | Tight | Primary story cards |
| Section Header | 20px–22px | 700 | Tight | Feed section titles |
| Body Large | 16px | 400 | 1.5 | Article body |
| Body Small | 14px | 400 | 1.45 | Supporting text |
| Metadata | 12px–13px | 400 | Normal | Timestamp/byline |
| Badge | 10px–12px | 700 | Tight | LIVE, weather, alerts |

## Principles

- Headlines should dominate hierarchy at all times
- Weight contrast is preferred over excessive size variation
- Typography should remain compact and scan-friendly
- Metadata should never visually compete with headlines
- Tight line-height is preferred for headline density
- Avoid decorative typography treatments or stylization

---

# 4. Component Stylings

## Buttons

### Watch Live CTA

- Background: `#D20F26`
- Text: `#FFFFFF`
- Radius: `4px`
- Height: `44px`
- Font Weight: `700`
- Use: Primary live streaming action

### Secondary Action

- Background: `transparent`
- Border: `1px solid rgba(255,255,255,0.16)`
- Text: `#FFFFFF`
- Radius: `8px`

### Topic Follow Button

- Background: `#19305F`
- Text: `#FFFFFF`
- Radius: `999px`
- Use: Follow/tag interactions

## Cards & Containers

- Background: `#19305F`
- Radius: `8px–12px`
- Dense vertical spacing
- Elevated subtly against deep navy background
- Cards should prioritize content hierarchy over decoration

## Live Video Module

- Full-width video surface
- Persistent LIVE badge
- Minimal chrome
- Expand/fullscreen action bottom-right
- Overlay gradients used for text readability

## Trending Stack

- Numbered circular ranking indicators
- Compact headline rows
- Minimal divider usage
- Dense scannable layout

## Inputs

- Background: `#223B72`
- Text: `#FFFFFF`
- Radius: `8px`
- Border: `rgba(255,255,255,0.12)`
- Focus state: FOX Blue border emphasis

---

# 5. Layout Principles

## Spacing System

- Base unit: `8px`
- Scale: `4px, 8px, 12px, 16px, 24px, 32px, 48px`

## Feed Architecture

The feed should contain a mixture of:
- Hero stories
- Live video modules
- Weather modules
- Trending lists
- Horizontal video rails
- Dense headline stacks
- Local + national story blending

Avoid repetitive layouts for long stretches. The feed should feel editorially curated and continuously updating.

## Whitespace Philosophy

- Content density is prioritized over excessive breathing room
- Dark backgrounds provide visual separation instead of large spacing gaps
- Every screen should maximize information utility without feeling cluttered
- Scanning speed is more important than visual minimalism

## Border Radius Scale

- Minimal (`2px`) — LIVE badges
- Small (`4px`) — Utility buttons
- Standard (`8px`) — Cards and modules
- Comfortable (`12px`) — Hero surfaces
- Pill (`999px`) — Follow chips and tags

---

# 6. Depth & Elevation

| Level | Treatment | Use |
|---|---|---|
| Base | `#042152` | Application background |
| Surface | `#19305F` | Standard cards/modules |
| Elevated | `rgba(0,0,0,0.24) 0px 4px 12px` | Hover/elevated surfaces |
| Modal | `rgba(0,0,0,0.45) 0px 12px 32px` | Dialogs/menus |
| Overlay | `rgba(4,33,82,0.92)` | Floating navigation/menus |

## Shadow Philosophy

FOX LOCAL uses restrained shadows compared to entertainment apps. Elevation should feel functional and newsroom-grade rather than cinematic or floating. Shadows exist primarily to preserve separation and readability across dense dark layouts.

---

# 7. Do’s and Don’ts

## Do

- Prioritize information density
- Use strong editorial hierarchy
- Keep layouts compact and scan-friendly
- Reserve FOX Red for urgency and live states
- Design mobile-first by default
- Use modular feed composition
- Maintain fast and functional interactions

## Don’t

- Don’t introduce playful or social-media-style aesthetics
- Don’t use glassmorphism or blurred translucent UI
- Don’t use oversized whitespace
- Don’t overuse FOX Red decoratively
- Don’t introduce gradients as decoration
- Don’t use soft/pastel color palettes
- Don’t make layouts feel entertainment-first

---

# 8. Responsive Behavior

| Breakpoint | Width | Behavior |
|---|---|---|
| Mobile Small | `<390px` | Compact stacked feed |
| Mobile | `390px–576px` | Standard mobile layout |
| Tablet | `576px–768px` | Expanded modules |
| Tablet Large | `768px–1024px` | Multi-column support |
| TV / CTV | `1024px+` | 10-foot viewing optimization |

## Responsive Principles

- Mobile-first layouts should always be assumed
- Hero content scales proportionally
- Livestream modules maintain visual dominance
- Dense information hierarchy preserved at all breakpoints
- Horizontal carousels expand progressively on larger screens

---

# 9. Agent Prompt Guide

## Quick Color Reference

- Background: `#042152`
- Surface: `#19305F`
- Text: `#FFFFFF`
- Secondary Text: `#8A9BB8`
- Accent Red: `#D20F26`
- Accent Blue: `#4378D4`

## Example Component Prompts

- “Create a FOX LOCAL breaking news card with deep navy background, 12px radius, bold white headline, muted timestamp, and FOX Red LIVE badge.”
- “Design a dense mobile news feed with mixed hero stories, trending stacks, weather modules, and horizontal video rails.”
- “Build a livestream module with minimal chrome, persistent LIVE indicator, fullscreen action, and overlay headline.”
- “Create a scan-friendly article detail view with large headline, muted metadata, The Brief bullet section, and full-width media.”

## Iteration Guide

1. Start with deep navy (`#042152`) as the foundational canvas
2. Prioritize headline hierarchy above all else
3. Use FOX Red only for urgency/live emphasis
4. Keep spacing dense and information-forward
5. Motion should feel operational, not decorative
6. Build modular editorial layouts optimized for continuous scrolling
```
