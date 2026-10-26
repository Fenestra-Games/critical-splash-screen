# Changelog

## 2.10.0

- Rebranded as a Fenestra Games module, with an MIT licence.
- The manifest now declares `type`, `license`, `readme`, `bugs`, `changelog`, `styles`, and `media`.
- Settings windows use a shared stylesheet (`styles/critical-splash-screen.css`) with section cards and a row layout that matches DND QuickPay.
- Added a README and wiki documentation.
- All settings text now comes from `lang/en.json`, so the module can be translated.
- The default crit and fumble images now point at the bundled `DefaultCritP4.webp` and `DefaultFumbleP4.webp`.

## 2.9.1

- Per-character setup and global settings are now two separate menus.
- Characters are added by dragging an actor in or pasting an Actor UUID.
- Crit and fumble sounds play independently of the splash image.
