# Ad SDK remote config

`config.json` is read by the game at every launch.

- `enabled`: `false` turns the SDK off completely (no ads requested, Show() just reports Failed).
- `adUnitId1/2/3`: real AdMob waterfall ad units. Leave `""` to keep the ones baked into the game.

Push to `main` to apply. GitHub's raw CDN caches ~5 minutes.
Game-side URL: `https://raw.githubusercontent.com/<user>/<this-repo>/main/config.json`
(this repo must be PUBLIC; never put secrets here - ad unit ids are not secret).
