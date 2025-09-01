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
  - Subtle grid background; dashed reticle; focus ring via `--ring`.

## Components

- Panels: `.panel` with `.panel__header`, `.panel__title`, `.panel__meta`, `.panel__body`.
- Navigation: `.hud-nav` with `.nav-list` and `.nav-link` using section anchors.
- Tags: `.tag`, muted variant `.tag--muted`.
- Stats: `.stat` pairs (`.stat__k`, `.stat__v`) for compact readouts.
- Lists: `.list` + `.list__row` for publications or items with meta.
- Contact: `.contact` with two-column `.contact__row`.
- Reticle: `.fx-reticle` overlay (purely decorative, subtle).

## Customize

- Accent color: update `--accent` in `styles.css`.
  - Examples: cyan `#7ae1ff`, amber `#ffd65c`, lime `#a5ff6b`.
- Name and role: edit `.hud-brand__name` and `.hud-brand__role` in `index.html`.
- Sections: duplicate or remove any `.panel` block as needed.
- Fonts: switch to `--sans` if you prefer a non-mono look.

## Accessibility

- High-contrast palette on dark background.
- Visible focus styles (`:focus-visible`).
- Skip link to main content.
- Reduced motion honored via `prefers-reduced-motion`.

## Layout & Responsiveness

- Desktop: two-column with sticky nav.
- Mobile: nav becomes a top block; content stacks; contact rows collapse to single column.

## Notes

- No JavaScript by design; UTC/year placeholders are static text.
- Keep content concise to maintain the utilitarian feel.

## Deploy

- Host as static files anywhere (e.g., GitHub Pages, Netlify, S3). Just upload `index.html` and `styles.css`.
