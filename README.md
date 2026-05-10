# Itoshima Sounds

<img src="images/headerrepo.jpg" style="zoom:50%;" />

## Overview

A minimalist Itoshima sound experience with scheduled farm chimes plus an optional experimental climate-reactive Koto layer.

## Core Experience

- Clean main interface (clock + ON/OFF + background image)
- Images rotate every 5 minutes
- Scheduled audio events at 07:00 / 12:00 / 17:00
- Manual triggers via keys (`1`, `2`, `3`)

## Sidebar Sound Lab (Collapsible)

A right-side hidden-by-default sidebar adds live Itoshima climate data and musical controls:

- Temperature
- Wind
- Humidity
- Precipitation
- Weather code
- Current sonic scene
- Active scale (Hirajoshi / Insen / Yo)

## Koto Climate Engine

When audio is ON, a generative WebAudio Koto-like layer runs in the background.

Climate mapping:

- Temperature -> pitch register
- Humidity -> reverb amount
- Precipitation -> delay time
- Wind -> phrase density / voices
- Day period -> scale family

Musical rules:

- Morning: Hirajoshi
- Noon: Insen
- Evening/Night: Yo
- Limited voices for long-running listening comfort

## Config Files

- `config/itoshima.config.yaml` (default)
- `config/itoshima.config.json` (fallback)

Main folders:

- `audio/` for playable tracks
- `img/` for rotating backgrounds

## GitHub Pages

GitHub Actions workflow is included:

- `.github/workflows/pages.yml`

To publish:

1. Push to `main`
2. GitHub -> `Settings` -> `Pages`
3. Select `Source: GitHub Actions`
4. Wait for `Deploy Static Site to GitHub Pages`

## References

- https://studiokura.info/en/
- https://en.wikipedia.org/wiki/Itoshima,_Fukuoka
