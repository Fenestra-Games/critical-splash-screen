# Critical Splash Screens

Show a per-character splash image and play a sound on natural 20s and natural 1s in Foundry VTT, with lowered crit thresholds and a random death sound.

> [!IMPORTANT]
> **AMEND:** Add a banner screenshot or a short GIF of a crit splash here. Suggested size: about 900 px wide.

![Banner placeholder](docs/banner.png)

- **Foundry:** v11 or newer, verified on v14
- **System:** dnd5e
- **Requires:** [Sequencer](https://foundryvtt.com/packages/sequencer)
- **Licence:** MIT
- **Author:** Fenestra Games (support@fenestra.gripe). Made using Claude AI.

Full documentation is in the [wiki](https://github.com/Thriceisalways/critical-splash-screen/wiki).

## What it does

- Shows a static image over the whole screen on a crit or fumble, for every connected player, regardless of vision or fog.
- Works for attack rolls, death saving throws, ability checks, and skill checks.
- Each character can have their own crit and fumble image and sound. The image is chosen by the character that rolled, so it still works when the GM rolls for a player.
- Default images and universal sound folders cover any character you have not set up.
- Lowered crit thresholds (for example Improved Critical) are detected from the character sheet, or set by hand.
- Plays a random sound from a folder when a token gets the "dead" status.
- Runs on the GM's client only, so connected players never layer their own random sounds on top of each other.

## Install

1. In Foundry, open **Add-on Modules, Install Module**.
2. Paste this into **Manifest URL**: `https://github.com/Thriceisalways/critical-splash-screen/releases/latest/download/module.json`
3. Install **Sequencer** as well.
4. Enable both in your world.

> [!IMPORTANT]
> **AMEND:** If you later list the module in the Foundry package directory, replace this section with a link to the package page. The directory description must be written by a human.

## Quick start

1. Open **Configure Settings, Module Settings, Critical Splash Screens**.
2. In **Global Settings**, set the screen scale, the default crit and fumble images, and your sound folders.
3. In **Per-Character Setup**, drag an actor onto a row (or paste an Actor UUID) and choose their images and sounds.
4. Roll a natural 20 and enjoy.

> [!IMPORTANT]
> **AMEND:** Add a screenshot of the Per-Character Setup window with two characters filled in.

## Documentation

| Page | What is in it |
| --- | --- |
| [Installation](https://github.com/Thriceisalways/critical-splash-screen/wiki/Installation) | Install, requirements, updating |
| [Global settings](https://github.com/Thriceisalways/critical-splash-screen/wiki/Global-settings) | Scale, default images, sound folders |
| [Per-character setup](https://github.com/Thriceisalways/critical-splash-screen/wiki/Per-character-setup) | Adding characters, images, sounds |
| [Crit thresholds](https://github.com/Thriceisalways/critical-splash-screen/wiki/Crit-thresholds) | Improved Critical and manual overrides |
| [Sounds and folders](https://github.com/Thriceisalways/critical-splash-screen/wiki/Sounds-and-folders) | Custom sounds, fallbacks, death sounds |
| [FAQ and troubleshooting](https://github.com/Thriceisalways/critical-splash-screen/wiki/FAQ-and-troubleshooting) | Common problems |

## Known limitations

> [!IMPORTANT]
> **AMEND:** Review this list before release and update it if anything has changed.

- **GM must be online:** all effects are triggered from the GM's client. If no GM is connected, nothing plays.
- **dnd5e only:** roll detection reads dnd5e chat message flags.
- **Settings are world settings:** they hold no secrets, but a player who reads the console can see the image paths.
- **Tested in one world:** please report anything odd, especially with other roll-automation modules.

## Reporting problems

Open an issue at https://github.com/Thriceisalways/critical-splash-screen/issues, or email support@fenestra.gripe. Please include your Foundry version, the module version, and any red console errors.

> [!IMPORTANT]
> **AMEND:** Decide whether you want a support Discord or a Ko-fi/Patreon link here.

## Licence

MIT. See [LICENSE](LICENSE).
