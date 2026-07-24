# kpop-theme

A dark [Spicetify](https://spicetify.app/) theme with neon K-pop
themed accents

## Features

- **Holographic glass UI** — sidebar, right sidebar, top bar, cards and
  tooltips use a frosted `backdrop-filter` blur with soft borders.
- **Flicker-free playbar** — the now-playing bar intentionally uses a solid
  gradient instead of `backdrop-filter`, avoiding the per-frame repaint
  flicker that a blurred, constantly-updating progress bar would otherwise
  cause.
- **Neon accents** — Electric Lilac `#C9A6FF`, Holographic Pink `#FF4FD8`
  and Cyber Cyan `#6BE7FF`, used for glows, active states, the progress bar
  and the scrollbar.
- **Custom play buttons** — Spotify green is fully replaced with the theme's
  pink accent; play buttons stay hidden until you hover a card or track row.
- **Custom typography** — [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk)
  for body text, [Syne](https://fonts.google.com/specimen/Syne) for headings.

## Installation

1. Make sure [Spicetify](https://spicetify.app/docs/getting-started) is
   installed.
2. Clone this repo into your Spicetify `Themes` folder as `kpop-theme`:

   ```sh
   git clone https://github.com/Chrisss666/kpop-theme.git "$(spicetify -c | xargs dirname)/Themes/kpop-theme"
   ```

   Or manually copy `color.ini` and `user.css` into
   `<spicetify config dir>/Themes/kpop-theme/`.

3. Apply the theme:

   ```sh
   spicetify config current_theme kpop-theme
   spicetify apply
   ```

## Customization

- Colors are defined once in [`color.ini`](color.ini) and consumed as
  `--spice-*` variables — tweak the `[Base]` section to
  change the palette without touching the CSS.
- Theme-specific tuning (glass opacity, blur radius, glow strength, corner
  radius, fonts) lives in the `:root` custom properties and section 1 of
  [`user.css`](user.css).

## License

[MIT](LICENSE) © Chrisss666
