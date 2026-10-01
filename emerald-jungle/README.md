# Emerald Jungle — v1.1

A dark emerald theme with gold accents for Hydra Launcher.

- Palette: base `#0a0f0c` / `#12241b`, emerald `#1db980` → `#12996a`, gold `#e0b64a`.
- Frosted-glass section headers, gold markers on active items, emerald hover states.
- Taller hero banner (500px) on game and profile pages — adjustable, see below.
- Achievement sound: `achievement.wav` (Hydra's default sound).

Built for vanilla Hydra. A few rules target features of the
[sotik11/hydra](https://github.com/sotik11/hydra) fork (localizations, the all-badges
modal, localization sources, the earned-points progress bar) — on vanilla those
selectors simply match nothing.

## Install

1. Copy `theme.css`.
2. In Hydra: **Settings → Appearance → Create**, name it `Emerald Jungle`, paste the CSS, save.
3. Optional: in the theme editor, upload `achievement.wav` as the achievement sound.

## Customize

The adjustable values sit at the very top of `theme.css`:

```css
:root {
  --ej-game-banner-height: 500px;       /* game page banner */
  --ej-profile-banner-height: 500px;    /* profile banner */
  --ej-button-radius: 999px;            /* button corners; 999px = pill */
  --ej-profile-button-padding-y: 18.5px; /* sidebar profile block height */
}
```

Change the numbers, save the theme, done.

## Store (hydrathemes.shop)

Themes reach the store through a pull request to
[hydralauncher/hydra-themes](https://github.com/hydralauncher/hydra-themes), as a folder
`themes/Emerald Jungle-<friend code>/` with:

- `theme.css`
- `screenshot.png` (or jpg, jpeg, webp, avif, heic, heif)
- `achievement.wav` (optional; Hydra also accepts mp3, ogg, m4a)

The store's validation checks that the friend code belongs to a real Hydra user and that
the theme name is unique. The site serves the theme under its lower-cased name
(`emerald jungle`), which is where Hydra fetches `theme.css` and the achievement sound from.
