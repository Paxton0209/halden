# Halden

An open-source HMI and interface sans-serif typeface tuned for automotive cockpits, design tools, and quiet editorial clarity.

**Live Specimen:** https://paxton0209.github.io/halden/  
**Release:** [Download Halden v1.0.0 (TTF + WOFF2)](https://github.com/Paxton0209/halden/releases/latest)

## Design Intent

Halden blends crisp neo-grotesque structure with restrained superellipse breathing room (`x-height / cap = 0.736`, `opsz = 20`), designed to stay calm at `letter-spacing: 0em` across light editorial pages and dark OLED cockpit displays:

- **Three calibrated weights**: `Regular (400)`, `Medium (500)`, `SemiBold (600)` with clear optical hierarchy (`n` stem `81 → 103.5 → 122.5`).
- **Disambiguated defaults baked in**: single-story `a`, single-story `g`, restrained bottom-hook `l` (zero `I / l / 1` ambiguity in 2-second glances), and open `3 / 4 / 6 / 9` numerals.
- **Contextual optical alignment (`calt`)**: colons (`08:45`, `12:54`) and hyphens/en-dashes (`2026-0417`, `08:45–17:30`) automatically center vertically between numerals.
- **Zero collisions**: full Latin coverage (2,933 glyphs per weight) with verified collision-free kerning.

## Quick Usage (Web)

```css
@import url("./fonts.css");

:root {
  font-family: "Halden", -apple-system, BlinkMacSystemFont, sans-serif;
  font-feature-settings: "calt" 1;
  letter-spacing: 0em;
}
```

## Files

- `ttf/` — Desktop TrueType fonts (`Halden-Regular.ttf`, `Halden-Medium.ttf`, `Halden-SemiBold.ttf`)
- `webfonts/` — Web-optimized WOFF2 fonts
- `fonts.css` — Ready-to-use `@font-face` stylesheet
- `OFL.txt` — SIL Open Font License 1.1
- `FONTLOG.txt` — Provenance, build metrics, and glyph modification log

## License

Licensed under the [SIL Open Font License 1.1](OFL.txt). Free for personal, commercial, web, desktop, and automotive HMI embedding. Built as an OFL derivative of Inter with parametric optical fitting, default alternate baking, custom `l`-hook restraint, and contextual `calt` vertical centering.
