# ProcureTEX Design System

Brand and social media asset guidelines for **ProcureTEX** — 3 November 2026 · Circa, Amsterdam.

---

## Brand at a glance

| Token | Value |
|---|---|
| Primary purple | `#6B35E8` |
| Deep navy | `#1A0A3C` |
| Lime accent | `#C8FF00` |
| Dark navy bg | `#0D0720` |
| Secondary text | `#B8A8E8` |
| Font | DM Sans (Google Fonts) |
| Visual motif | Circle/node/lattice dot grid |
| Event date | 3 November 2026 |
| Venue | Circa, Amsterdam |
| URL | procuretex.com |

**Rules:**
- Lime (`#C8FF00`) is an accent only — labels, CTAs, company names, highlights. Never use for body copy.
- Secondary text is always `#B8A8E8` — never grey, never white at reduced opacity.
- Logo: `ProcureTEX` — the `TEX` is always lime, `Procure` is always white.
- Backgrounds: always dark. Never white or light backgrounds.
- Speaker photos: right side with left-to-right gradient fade. Never circles — use `border-radius: 12–16px`.

---

## Asset templates

| File | Format | Use |
|---|---|---|
| `components/speaker-card.html` | 480×480px (1:1) | Single or multi-speaker LinkedIn posts |
| `components/partner-post.html` | 480×480px (1:1) | Community/proud partner announcements |
| `components/linkedin-banner.html` | 480×270px (16:9) | Event banners, session announcements |

---

## How to generate assets with Claude

Go to [claude.ai](https://claude.ai) and use these prompt templates. Paste the prompt, attach any photos needed, and Claude will output a ready-to-export HTML file.

---

### Speaker card (single)

```
Using the ProcureTEX brand system (deep navy/purple background #1A0A3C→#6B35E8 gradient, lime accent #C8FF00, DM Sans font, node/lattice dot pattern overlay), create a 480×480px LinkedIn speaker card for:

Name: [Full name]
Title: [Job title]
Company: [Company name]
Session: [Session title or leave blank]

Attach their headshot — place it on the right side with a left-to-right gradient fade. Add "Save your spot →" CTA button in lime and procuretex.com URL in the footer. Label pill should read "Speaker" in lime outline style.
```

---

### Multi-speaker card (3 speakers)

```
Using the ProcureTEX brand system (deep navy background #1A0A3C, lime accent #C8FF00, DM Sans font, node/lattice dot pattern), create a 480×480px LinkedIn speakers card with:

Speaker 1: [Name] · [Title] · [Company]
Speaker 2: [Name] · [Title] · [Company]
Speaker 3: [Name] · [Title] · [Company]

Session/panel title: [Title or leave blank]

List speakers vertically with small rounded headshots (52×52px, border-radius 12px, lime border at 25% opacity). Add "Save your spot →" CTA and procuretex.com in the footer.
```

---

### Partner post

```
Using the ProcureTEX brand system (deep navy/purple gradient background, lime accent #C8FF00, DM Sans font, node lattice pattern), create a 480×480px community partner post for:

Partner name: [Company name]
[Attach partner logo — will be placed white/inverted centre card]

Layout: ProcureTEX logo top-left, "Community Partners" label, partner logo centred, divider line in lime, "Proud partner of" in muted text, "ProcureTEX" in large bold type below with TEX in lime. Event date and procuretex.com in footer.
```

---

### LinkedIn banner (16:9)

```
Using the ProcureTEX brand system (deep navy/purple gradient #1A0A3C→#6B35E8, lime accent #C8FF00, DM Sans font), create a 480×270px LinkedIn banner for:

Headline: [2–4 words]
Subtext: [Speaker name, session title, or event detail]
CTA: [Register now / Save your spot / Learn more]
[Attach speaker photo if applicable]

Place photo right side with fade overlay. Add event label pill "3 Nov · Amsterdam" in lime outline above headline.
```

---

## Exporting

All templates are HTML files — open in Chrome, then:

1. Right-click → Inspect → toggle device toolbar
2. Set canvas to exact pixel dimensions
3. Use a screenshot tool (CleanShot, Shottr, or browser extension) to capture at 2× for retina export
4. Or: open the HTML, `Cmd+Shift+4` on Mac to screenshot the exact card area

For batch exports or higher fidelity, bring the HTML into Figma via the HTML-to-Figma plugin, or rebuild in Figma using these tokens.

---

## Adding new asset types

To add a new template, ask Claude:

```
Using the ProcureTEX design system in this repo (purple #6B35E8, lime #C8FF00, navy #1A0A3C, DM Sans, node lattice pattern), create a new [asset type] template at [dimensions]. Follow the same file structure as the existing components.
```
