---
name: zoom
description: Use when the user runs /zoom, or when attacking, auditing, tearing down, or rewriting vibecoded or AI-slop UI. Triggers: vibecoded, AI slop, demo banners, sample node pills, placeholder telemetry, mock tables, Lucide overload, purple-on-black, bento, 3 feature cards, liquid glass, fake testimonials, sparkle icons, neon gradients, Inter/Geist/Space Grotesk, missing ToS or privacy. Do not use for greenfield brand systems or non-UI work.
---

# Zoom

Tear down vibecoded / AI-slop UI. Do not install a replacement template.

## Yields

Apply before any ban:

- A committed design system, type stack, or icon set in the repo wins unless the user said tear it down.
- The brief and brand book win, including purple, white, glass, or three pricing plans.
- Marketing pages and product apps are different surfaces. Do not force landing-page structure onto dashboards.
- A tell that is doing a real job stays. Costume around empty content does not.

## Attack sequence

1. Name the surface: `marketing` | `product` | `mixed`.
2. Scan against the 34 tells below. Cite file and line (or a screenshot region) for each hit.
3. Emit the report. Do not start rewriting during the scan.
4. Rewrite only if asked. Strip first. Rebuild from real product content, not from an anti-slop kit.

**Do not** "fix" slop by shipping the same alternate kit every time (Satoshi / Plus Jakarta, `#F8F9FA`, 1px hairlines, `rounded-md`, editorial slate, one accent). Infer color, type, and layout from the product. If you cannot name why a choice belongs to this product, it is still slop.

## The 34 tells

Hit = the costume, not the legitimate version in **Keep**.

| # | Tell | Slop | Fix | Keep |
|---|---|---|---|---|
| 1 | Harsh gradients | Multi-stop neon or muddy fills on backgrounds or type | Solid surface or one-hue luminance shift | Documented brand gradient that still contrasts |
| 2 | Lucide icons | Icon on every heading, button, input, and card | Labels first; one family only if a glyph is needed | Product already standardized on Lucide and use is sparse |
| 3 | Pure white background | `#FFFFFF` void with no surface or ink hierarchy | Give surfaces a relationship (page / panel / ink). Off-white is one option, not the rule | Brand is paper-white on purpose |
| 4 | Rainbow coloring | A different bright accent on every card or tag | One accent. Semantic color only for success / danger / warning | Data viz or a real status system |
| 5 | Drop shadows | Large black blur (`shadow-xl`, 16px+ spread) | Hairline, tight tinted shadow, or nothing | Subtle elevation already in the design system |
| 6 | 3 feature cards in a row | Equal icon + title + blurb columns | Layout that matches the actual content (split, list, one focus band) | There are really 3 distinct things and the cards are not filler |
| 7 | Emojis | Emoji in titles, cards, or nav | Type and structure | Chat, social, or a playful product that already uses them |
| 8 | Liquid glass | `backdrop-filter` cards as the default surface | Solid, readable surfaces | Overlay / nav, and text still meets contrast |
| 9 | Em dashes | `—` as a voice tic in headlines and body | Period, comma, colon, or hyphen | Rare grammar, not a pattern |
| 10 | Inter / Geist / Space Grotesk | Unmodified default stack as the whole identity | Type that fits this product | Already committed in the repo |
| 11 | Colored left stripe | 3–4px accent border on cards or alerts | Tint, type weight, or a status chip | The design system specifies it |
| 12 | Fake testimonials | Invented names, roles, quotes, or vanity stats | Real evidence, or delete the section | Verifiable customers and quotes |
| 13 | Bento grids | Mixed rounded tiles hiding weak hierarchy | Structure that follows content priority | Cell count equals real items and sizes mean something |
| 14 | Terminal window | Fake traffic-light chrome around static code | Real screenshot, live snippet + copy, or delete | A working terminal or code sample the user can use |
| 15 | "It's not X, it's Y" | Contrast slogan instead of a claim | Say the capability in plain language | Never. Rewrite it. |
| 16 | Checkmark bullets | Green ticks as a feature list | Plain list or a comparison table | A real feature matrix |
| 17 | 3 pricing tiers | Free / Pro / Enterprise towers, tall middle, "Most Popular" | Comparison table or the real price. Three plans are allowed | Real tiers without the costume |
| 18 | No real product demos | Fake div dashboards, gradient-blob heroes | Real screenshot or working UI. If neither exists yet, cut the section | Live product or captured UI |
| 19 | Soft corner radius | `rounded-2xl` / `rounded-3xl` on every box | One radius scale. Tighter on large containers | A consistent soft scale already in the system |
| 20 | Purple and black | Violet / fuchsia / cyan glow on near-black | Neutrals + the product's actual accent | Brand is purple |
| 21 | No skeleton loaders | Blank flash or layout jump on fetch | Same-shape skeleton, plus empty and error | Instant / local-only UI |
| 22 | Radial orbs | Blurred color circles behind empty sections | Negative space or real imagery | None as decoration |
| 23 | Dot grids | Decorative dot / mesh / wireframe backgrounds | Nothing, or a texture that belongs to the brand | Brand pattern used with restraint |
| 24 | Sparkle icons | Sparkle / wand = "AI" | Name the capability | Never as a synonym for intelligence |
| 25 | Animated arrows | Bouncing / sliding arrows begging for a click | Still chevron, or none | None |
| 26 | No ToS | Public site footer links to `#`, or the link is missing | Real `/terms`, or remove the link | Not a public marketing surface |
| 27 | No privacy policy | Same for privacy | Real `/privacy`, or remove the link | Not a public marketing surface |
| 28 | Hover animations | Cards lift, tilt, float | Hover only on controls; color or border; `:active` press | Simple background / color hover on controls |
| 29 | Neon colors | High-sat accents that fail contrast | Lower chroma. Body text ≥ 4.5:1, UI chrome ≥ 3:1 | Brand neon that still passes contrast |
| 30 | Basic pastel colors | Generic mint / lilac / peach wash | Grounded tones taken from the product | Brand is pastel on purpose |
| 31 | Defensive demo banners | "Local demo", "Sample node", "Demo only", fixture-account pills on a product surface | Production chrome. Status can be operational. Do not apologize that the build is a demo | A staging flag the user asked to keep |
| 32 | Placeholder telemetry | Invented TPS, incrementing counters, random-hash live feeds, charts of fake weekly points | Zero placeholder telemetry. Bind the widget to a real feed, or omit it | Live data from an actual source |
| 33 | Arbitrary mock tables | HTML tables stuffed with invented rows to look full | Typed table that maps explicit records. No schema: remove the section | Tables driven by a declared schema and supplied rows |
| 34 | Loose numeric columns | Proportional figures left-aligned in tables | Right-align numeric columns. `font-variant-numeric: tabular-nums` | Non-numeric text columns |

## Report

```markdown
## Slop report
Surface: marketing | product | mixed
Hits: N/34

| # | Tell | Where | Keep? | Fix |
|---|---|---|---|---|
| 6 | 3 feature cards | `HeroFeatures.tsx:42` | no | one split + a list |

Rewrite order (only if asked): highest-visibility hits first. Delete fake evidence before restyling.
```

## Rewrite rules

- Strip decoration before adding anything.
- Do not swap one cliché for the next (interactive pricing slider, custom SVG icon set, "runnable API workbench") unless the product needs that object.
- Copy, states, and metrics must be factual. No fake metrics, no contrast slogans, no em-dash tic.
- Product UI looks like production. Strip demo banners and "sample node" pills. Do not invent a live network out of placeholders.
- Do not fill tables to look busy. Map a typed record list, or cut the section until a real schema exists.
- Numeric columns are right-aligned with tabular figures.
- Public marketing pages need working legal routes or no legal links. App-only surfaces do not grow a ToS page from this skill.
- After a rewrite, rescan the 34. New costume still counts as a hit.
