# Itoshima Sounds

Minimal interface + experimental Japanese generative sound lab driven by Itoshima climate.

## Main Experience

- Clock + ON/OFF button
- Rotating background images every 5 minutes
- Scheduled farm sounds at 07:00 / 12:00 / 17:00
- Manual triggers with keys: `1`, `2`, `3`

## Collapsible Sidebar (Sound Lab)

Hidden by default to keep the visual clean.

Includes:

- Live Itoshima climate metrics
- Instrument selector (5 voices): `Koto`, `Shamisen`, `Biwa`, `Shakuhachi`, `Taiko Bell`
- Reverb time
- Delay time
- Delay feedback
- Dry/Wet mix
- String layer volume
- Drone ON/OFF + drone volume

## Audio Engine

WebAudio generative engine:

- Climate to music mapping:
  - Temperature -> pitch register
  - Wind -> phrase density
  - Humidity -> wetness/reverb tendency
  - Precipitation -> delay character
- Time-of-day scale changes:
  - Morning: Hirajoshi
  - Noon: Insen
  - Evening: Yo

## Config

Primary config files:

- `config/itoshima.config.yaml` (default)
- `config/itoshima.config.json` (fallback)

Assets:

- `audio/`
- `img/`

## GitHub Pages

Workflow included:

- `.github/workflows/pages.yml`

To publish:

1. Push to `main`
2. `Settings` -> `Pages`
3. Set source to `GitHub Actions`
4. Wait for deploy workflow
## License

MIT License — © 2026 [Vladimiro Bellini](https://github.com/vlasvlasvlas). Free to use and modify, attribution required.
