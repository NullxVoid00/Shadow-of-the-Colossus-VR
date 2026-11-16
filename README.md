# Shadow of the Colossus VR

**In development · No public mod release yet · PC VR**

A first-person VR adaptation of **Shadow of the Colossus**, built around a modified PCSX2 runtime and an OpenXR bridge. Development focuses on reaching, climbing, bow handling, equipment and preserving the scale of the original world.

[Future downloads & release notes](https://github.com/NullxVoid00/Shadow-of-the-Colossus-VR/releases) · [Report an issue](https://github.com/NullxVoid00/Shadow-of-the-Colossus-VR/issues) · [Abyssal Light Games](https://nullxvoid00.github.io/)

## Release status

This is the public project and future release hub. **There is no downloadable mod build published here yet.** The repository currently contains project information and release documentation; GitHub's **Code → Download ZIP** downloads those documents, not an installable mod.

When a build is ready, its installer or archive, supported game version, controls, installation steps and known issues will be published under [Releases](https://github.com/NullxVoid00/Shadow-of-the-Colossus-VR/releases). Use **Watch → Custom → Releases** to follow future downloads. No release date is announced.

## What is being developed

| Area | Current development work |
| --- | --- |
| **First-person presence** | Stereo view transport, tracked hands/body posing, wrist HUD and authored cinematic handling are implemented in the development branch. |
| **Climbing experiments** | Independent hand contacts, grip transfers, jump/catch requests and moving-support transforms integrate with the native game motor and stamina rules. |
| **Equipment** | Shoulder weapon acquisition, physical bow draw/release with native arrow behavior, and a sword-raising gesture for native light are implemented. |
| **Setup** | A dedicated Windows launcher/installer supports a separate portable runtime, settings and checkpoint controls. |

## Target setup

- **Game / platform:** Windows PC; Shadow of the Colossus USA PS2 disc image (SCUS-97472 / CRC C19A374E), your own PS2 BIOS, and the project-specific runtime. This is not a PS3 or PS4 remake mod.
- **VR setup:** PC-connected OpenXR headset and tracked controllers. Quest 3 is the documented headset used during development. Personal reach/world-scale calibration is part of the setup.
- **Game ownership:** Supply your own required game files. No commercial game data, ROM, disc image, BIOS or save data is provided by this repository.

## Development controls

These are the current documented starting mappings, not a finalized release manual. The instructions shipped with a future build take precedence.

| Input | Action |
| --- | --- |
| Tracked grip near a supported surface | Request a climb contact / hold |
| Shoulder grip and extraction | Acquire a supported weapon |
| Bow-string grab, pull and release | Request a native bow shot |
| Raise sword above the head | Request native sword-light action |
| Ground grip + A | Native roll request; live verification remains pending |

## Known limitations and next work

- All 16 colossus encounters still require coverage. The first-colossus grabbing failure and unsupported collision geometry remain significant open work.
- Climbing movement still follows native animation-sized steps; it is not yet one-to-one physical climbing.
- Physical weak-point stabbing, stab depth/strength and tracked sword-light beam targeting are unfinished.
- Body/weapon fit, headset comfort and performance across demanding encounters remain unverified for the current build.

Builds, automated checks and desktop captures do not by themselves establish headset comfort, full-game compatibility or a release-ready experience. The descriptions above distinguish implemented development work from unfinished work.

## Installing a future release

Installation instructions will accompany each published build. Until then, there is no supported public installation procedure or binary to download from this repository. Game-version and runtime requirements may change as development continues.

## Feedback

Use [Issues](https://github.com/NullxVoid00/Shadow-of-the-Colossus-VR/issues) for questions or reports. For a future build, include its version, game version, headset/runtime and clear reproduction steps. Remove personal paths and private information from logs, and do not attach game files or saves.

## Credits

VR project by **NullxVoid / Abyssal Light Games**. This is an unofficial fan project and is not affiliated with or endorsed by the original game's creators or publishers.

- [PCSX2](https://github.com/PCSX2/pcsx2) — Emulation foundation for the project-specific runtime and game integration.

Original games, names and assets belong to their respective owners. Upstream code and dependencies retain their own licenses. Future distributions will include the applicable notices and source obligations; this documentation hub does not relicense upstream or game material.

## Maintaining releases

See the [release guide](docs/RELEASE_GUIDE.md) and [release notes template](docs/RELEASE_TEMPLATE.md).

*Project information reviewed 2026-11-16 against local development documentation. This date is not a release or headset-certification date.*
