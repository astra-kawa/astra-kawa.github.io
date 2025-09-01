# Personal Homepage — HUD Minimal Template

A modern, minimal, utilitarian homepage inspired by aircraft/spacecraft HUDs. Vanilla HTML + CSS, no JS or external fonts.

## Files

- `index.html`: Single-page layout with sections for Overview, Missions, Publications, Skills, and Contact.
- `styles.css`: Design tokens, layout, and HUD components.

## Design System

- Colors (CSS variables in `:root`):
  - `--bg`, `--surface`, `--line`, `--line-2`: Backgrounds and linework.
  - `--text`, `--muted`: Primary/secondary text.
  - `--accent`: HUD accent (green by default). Also `--ok`, `--warn`, `--err`.
- Typography:
  - System stacks only. Monospace primary (`--mono`) to echo avionics UIs.
  - Sizes: `--fs-1 … --fs-4`; line-height `--lh`.
- Spacing:
  - `--s-1 … --s5` (4–48px), 8px base scale.
- Effects:
  - Subtle grid background.

## Components

- Panels: `.panel` with `.panel__header`, `.panel__title`, `.panel__meta`, `.panel__body`.
- Tags: `.tag`, muted variant `.tag--muted`.
- Stats: `.stat` pairs (`.stat__k`, `.stat__v`) for compact readouts.
- Lists: `.list` + `.list__row` for publications or items with meta.
