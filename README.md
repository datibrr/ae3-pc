# Ape Escape 3 PC

**An unofficial reverse-engineering project for a native PC version of Ape Escape 3 (PlayStation 2) with Multiplayer Support.**

> **Project status: Early development - no public playable release.**
>
> This repository is an **information-only project page**. It currently contains no playable PC port, download, installer, source release, or setup instructions. This README explains the project's goals, internal development progress, and possible future features.

<img width="1920" height="1004" alt="ae3-pc" src="https://github.com/user-attachments/assets/e8af8519-802b-40bc-b944-4a60b74c848e" />

## About the Project

Ape Escape 3 PC is an experimental effort to reconstruct the original game's systems and run them natively on PC. The goal is a faithful single-player experience with keyboard and controller support, rather than running the PS2 game through an emulator.

The work is still at an early stage. Some parts of the game have been reconstructed or demonstrated in internal prototypes, but many systems are incomplete, use temporary approximations, or have not been fully integrated. **There is currently no complete or reliably playable PC version available to the public.**

The initial target platform is **Windows**. Additional PC features and multiplayer are longer-term possibilities; finishing the original single-player experience comes first.

## Development Progress

**Last updated:** October 15, 2026  
**Estimated overall progress:** ~40% toward a complete, faithful single-player port  

These percentages are rough development estimates, **not measured source-code coverage**. They represent how close each area is to a complete, integrated, and verified implementation. The overall figure is not an average of the individual categories: missing gameplay systems weigh more heavily than completed research or asset-import work.

### What Has Been Explored Internally

Internal development and testing have reached several milestones:

- A native Windows application using **C++** and a **Direct3D 11** renderer.
- Reading original disc archives and displaying most of the game's models, textures, and other assets.
- Early versions of the title screen, character selection, hub, and multiple game areas.
- Basic character movement, jumping, gadget interactions, and monkey-catching mechanics.
- Several camera behaviors, HUD elements, world selection, shop screens, and results screens.
- Initial work on progression, saving, music, sound, and video playback.
- Keyboard and XInput controller input with configurable bindings.
- Experimental split-screen and network prototypes.

### Detailed Progress Estimates

| Area | Estimated progress | Current state / remaining work |
| --- | --- | --- |
| Disc data and resource formats | 90% | Many formats have been decoded and checked; edge cases and full integration remain. |
| Native runtime and architecture | 70% | An internal Windows runtime exists; resource management and original systems still need work. |
| Graphics, models, and textures | 65% | Many scenes render; materials, lighting, water, transparency, and visibility need refinement. |
| Keyboard and controller input | 80% | Basic input and remapping exist; complete gameplay verification and edge cases remain. |
| Player movement and physics | 60% | Core movement and some reconstructed routines exist; collisions and state transitions need work. |
| Animation and gadget attachment | 50% | Original animation data is being used; transitions, character details, and special states remain incomplete. |
| Cameras | 65% | Several original camera behaviors have been reconstructed; scripted and special-case cameras remain. |
| HUD, menus, and screens | 75% | Many interfaces are present internally; animations, effects, and complete interactions need refinement. |
| Music, sound, and voices | 60% | Native playback is partially implemented; event timing and voice assignments need verification. |
| Gadgets and transformations | 40% | Some basic behavior exists; full mechanics, animation, and state handling remain unfinished. |
| Monkey AI | 30% | Some original data and reaction routines have been reconstructed; complete AI integration is still missing. |
| Enemies and bosses | 25% | Early placeholder behavior exists; original attacks, state machines, and fight phases remain incomplete. |
| Collisions, doors, switches, and moving objects | 55% | Foundational systems exist; behavior must be checked and completed across individual areas. |
| Progression, world selection, and saving | 65% | Early save and progression systems exist; complete story progression and edge cases remain. |
| Particles and special effects | 55% | Some effect data and rendering paths have been explored; triggering and timing are incomplete. |
| Full playthrough, testing, and performance | 25% | Individual tests exist, but complete playthrough validation and performance work remain. |
| Optional multiplayer | 25% | Split-screen and networking experiments exist; functional co-op and real-world networking are not complete. |

These estimates describe **development maturity, not public availability**. Reconstructed code that has not been integrated into gameplay is not counted as a finished gameplay feature, and none of these figures should be used to predict a release date.

## Priorities and Future Plans

### Faithful Single-Player Experience

The main priority is to recreate the original Ape Escape 3 single-player experience as accurately as possible. This includes movement, gadgets, monkey behavior, enemies, bosses, world progression, presentation, and the overall flow of the game.

The project also aims to support native PC resolutions, adjustable display settings, and customizable keyboard/controller controls. Some of these ideas already exist in experimental form, but they are **not finished public features**.

### Optional Local Co-op and Online Multiplayer

The Multiplayer co-op implementation allows players to explore the same area together, with separate cameras, HUD elements, health, energy, and gadget selections. The intention is to support local play on one PC and, eventually, play across multiple computers while keeping the original single-player mode intact.

Player synchronization, shared progression, saving, interactions, and full-game compatibility would all need substantial additional work.

### Other PC Enhancements

Because the intended result is a native PC application, further enhancements could eventually include quality-of-life options, alternative controls, custom game rules, additional gadgets, custom levels, or modding support.

## Original Game Data

The project does **not** distribute the original game or its copyrighted assets. Any future usable version is intended to rely on game data supplied by the user from their own copy of Ape Escape 3.

Current research is based on the **European PlayStation 2 release (SCES-53642)**. Support for other regions or disc revisions has not been confirmed.

Original models, textures, animations, music, scripts, and other game content are not provided here. No ISO, PS2 BIOS, or original game files are available through this repository.

**There is no public build or disc-import process to use at this time.** This section explains the project's intended approach, not installation steps.

## About This Repository

This GitHub repository is currently intended **only to share information about the project and its development progress**. This README is the complete public project overview here; there are no additional documentation pages, downloads, or build instructions to follow.

Progress information may be updated as development continues.

## Disclaimer

This is an unofficial fan project and is not affiliated with, sponsored by, or endorsed by Sony Interactive Entertainment. **Ape Escape** and all original game content belong to their respective rights holders.
