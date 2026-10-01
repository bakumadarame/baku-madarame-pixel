# Baku Madarame

A tiny pixel companion inspired by **Baku Madarame from Usogui**: tousled white hair, blue eyes, a white suit, and a red tie.

An unofficial fan-made pet for Codex. Artwork and animation frames were generated with OpenAI ImageGen, assembled into a sprite atlas, and checked for animation consistency and clean transparent edges.

| Idle | Hello | Jump |
| :---: | :---: | :---: |
| ![Idle](previews/idle.gif) | ![Waving](previews/waving.gif) | ![Jumping](previews/jumping.gif) |

## What's included

- Nine animation states: idle, moving right, moving left, waving, jumping, failed, waiting, working, and review.
- Sixteen look directions.
- A transparent **v2 sprite atlas**, 1536 × 2288 pixels.
- Two pet files: `pet.json` and `spritesheet.webp`.

## Install in Codex

Requires a Codex desktop version that supports custom pets.

1. Download `pet.json` and `spritesheet.webp` from this repository.
2. Create a folder named `baku-madarame-pixel` inside your user account's `.codex/pets` folder.
3. Place both files directly inside that folder.
4. Select **Baku Madarame** in Codex's pet picker. If it does not appear, restart Codex.

On Windows, the destination is `%USERPROFILE%\.codex\pets\baku-madarame-pixel`. On macOS and Linux, it is `~/.codex/pets/baku-madarame-pixel`.

This package contains an image and a JSON manifest. It includes no executable installer, scripts, account credentials, or application configuration changes. Menu placement and custom-pet support may vary by app version.

## All animations

The previews below show the complete set of states. They are demonstrations; the downloadable `spritesheet.webp` contains the full atlas, not just the three previews at the top of this page.

| State | Preview |
| :--- | :---: |
| Idle — breathing and blinking | ![Idle](previews/idle.gif) |
| Move right | ![Move right](previews/running-right.gif) |
| Move left | ![Move left](previews/running-left.gif) |
| Waving — greeting gesture | ![Waving](previews/waving.gif) |
| Jumping | ![Jumping](previews/jumping.gif) |
| Failed — error reaction | ![Failed](previews/failed.gif) |
| Waiting | ![Waiting](previews/waiting.gif) |
| Working — the `running` state | ![Working](previews/running.gif) |
| Review | ![Review](previews/review.gif) |

Which state plays, and when it plays, is controlled by the host app. Petdex and Codex may use different playback timings or frame counts. The package preserves every populated atlas cell from the installed pet.

## Look directions

![Sixteen look directions](previews/look-directions.gif)

## Quality checks

See [QUALITY.md](QUALITY.md) for package completeness, validation results, and known limitations. Sanitized build reports are available in [quality-checks](quality-checks/). Private build paths, account identifiers, and chat history are excluded.

## Credits and use

Pet package prepared by **Neumann**. See [ATTRIBUTION.md](ATTRIBUTION.md) for the fan-work attribution.

The contributor's licensable contributions to this package are licensed under **Creative Commons Attribution 4.0 International (CC BY 4.0)**. You may share and adapt those contributions, including commercially, under the license terms. When sharing, retain attribution to Neumann, link to the license, and indicate changes.

See [LICENSE.md](LICENSE.md) for the license notice and scope. The license does not grant rights to Baku Madarame, Usogui, or other third-party material, and does not create copyright in AI-generated material where no such rights exist.
