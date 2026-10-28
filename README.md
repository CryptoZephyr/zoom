# zoom

zoom is an agent skill that checks a web UI for the signs of "vibecoded" or AI-generated design and tells you what to cut. It's for developers who build with Claude Code, Codex, Cursor or similar agents and want their product to look like a real product, not a template.

Point your agent at a landing page or app and ask for `/zoom`. It scans the code against 34 common tells, such as fake testimonials, invented live stats, neon gradients on black, sparkle icons standing in for "AI", and a row of three identical feature cards. You get a report that cites the file and line for each hit. Nothing is rewritten unless you ask.

## What a report looks like

This sample shows the format for a made-up landing page:

```markdown
## Slop report
Surface: marketing
Hits: 4/34

| # | Tell | Where | Keep? | Fix |
|---|---|---|---|---|
| 12 | Fake testimonials | `Testimonials.tsx:8` | no | Delete the section until there are real customers |
| 32 | Placeholder telemetry | `Hero.tsx:51` | no | Remove the ticking "requests served" counter |
| 6 | 3 feature cards | `Features.tsx:20` | no | One split section plus a plain list |
| 24 | Sparkle icons | `Nav.tsx:14` | no | Name the feature instead of using a sparkle |

Rewrite order (only if asked): highest-visibility hits first. Delete fake evidence before restyling.
```

## It respects real design choices

Every tell has a "Keep" case. If your repo already has a design system, or your brand really is purple or uses glass, zoom leaves it alone. It only flags the costume: decoration that covers empty or invented content. It also won't swap one stock look for another. Fixes come from the product's own content.

## Install

zoom is a single `SKILL.md` file. Copy the `skills/zoom` folder into your agent's skills directory:

| Agent | Location |
|---|---|
| Claude Code | `~/.claude/skills/zoom/` |
| Codex | `~/.codex/skills/zoom/` |
| Other agents | Wherever your agent loads `SKILL.md` skills from |

```bash
git clone https://github.com/CryptoZephyr/zoom
cp -r zoom/skills/zoom ~/.claude/skills/
```

## Use

- `/zoom` or "audit this UI for AI slop" runs the scan and returns the report.
- "Rewrite it" after the report strips the hits, starting with the most visible ones, then rescans.

zoom is for auditing existing UI. It doesn't create a brand or design system from scratch.

## The 34 tells

The full list, with what counts as slop, the fix, and when to keep it, is in [skills/zoom/SKILL.md](skills/zoom/SKILL.md).

## License

MIT
