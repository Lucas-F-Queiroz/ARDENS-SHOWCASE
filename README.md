# ARDENS

> A pixel-art idle/AFK game about raising, progressing and managing dragons — built in Unity and developed as an evolving personal software project.

![Status](https://img.shields.io/badge/status-MVP%20complete-success)
![Current focus](https://img.shields.io/badge/current%20focus-visual%20rework-blueviolet)
![Engine](https://img.shields.io/badge/engine-Unity-black)
![Language](https://img.shields.io/badge/language-C%23-512BD4)
![AI assisted](https://img.shields.io/badge/development-AI%20assisted-6f42c1)

## Overview

ARDENS is a personal game project developed in Unity with C#. The project already has a functional MVP and is currently going through a broader visual rework focused on consistency, readability and a stronger art direction.

The project is also an ongoing exercise in software engineering: designing systems that can evolve, keeping scope under control, refactoring existing code, documenting decisions and using AI tools without giving up technical ownership.

The full source code is maintained privately. This public repository exists as a technical showcase of the project, its architecture, development process and selected implementation details.

## Current status

- Functional MVP completed
- Core gameplay loop implemented
- Ongoing visual and UX rework
- Existing systems being reviewed and refactored where needed
- Art direction and interface consistency being standardized
- Documentation being improved alongside development

## What I work on in this project

ARDENS is not only a game prototype. It is the project where I practice maintaining a growing codebase and making technical decisions over time.

Areas explored include:

- Gameplay and progression systems
- State and data management
- Inventory and economy-related systems
- UI flows and feedback
- Save/persistence concerns
- Code organization and refactoring
- Scope control and iterative delivery
- Documentation
- Visual consistency across a 2D pixel-art interface

## Development with AI

AI is part of the development workflow, especially OpenAI Codex.

I use it as an engineering tool for:

- Investigating existing code before changing it
- Planning changes across multiple files
- Implementing and iterating on features
- Reviewing code and spotting duplication
- Refactoring systems after the MVP stage
- Maintaining documentation
- Creating structured prompts for visual-asset workflows
- Comparing implementation alternatives

Generated suggestions are not accepted blindly. Changes are reviewed against the project context, tested inside Unity and adjusted when necessary.

The goal is to use AI to increase iteration speed while preserving ownership of architecture, product decisions and technical validation.



## Architecture

The public documentation intentionally stays at a high level because the production source remains private.

The project is organized around independent gameplay responsibilities instead of placing unrelated behavior into large scene scripts.

```text
Gameplay
├── Progression
├── Economy
├── Inventory
├── Dragon systems
└── Interaction rules

Presentation
├── UI screens
├── HUD / feedback
├── Navigation
└── Visual state

Data
├── Runtime state
├── Configuration
└── Persistence

Infrastructure
├── Save/load
├── Shared services
└── Development tooling
```

The exact structure evolves as the project is refactored.

More details: [`docs/ARCHITECTURE.md`](docs/ARCHITECTURE.md)

## Visual rework

The MVP proved the core systems, but it also made inconsistencies in the visual language more obvious.

The current rework focuses on:

- A consistent pixel-art direction
- Better hierarchy and readability
- Less visually forced UI composition
- Reworking dragon presentation where necessary
- Standardized spacing, scale and interface patterns
- Making assets feel like parts of the same game rather than isolated pieces

### Before / after

Screenshots and GIFs will be added here as the rework progresses.

| Before | After |
| --- | --- |
| `assets/screenshots/before.png` | `assets/screenshots/after.png` |

## Selected technical notes

Instead of publishing the complete Unity project, this repository can contain small, isolated examples that are safe to share.

See [`code-samples/README.md`](code-samples/README.md).

Planned examples:

- A small state/progression component
- A UI update flow
- A persistence-related example
- A refactoring example showing before/after reasoning

These samples should be understandable on their own and must not depend on proprietary assets.

## Engineering decisions

Some principles used while evolving the project:

1. **MVP first** — validate the loop before spending heavily on polish.
2. **Refactor after evidence** — restructure code when real usage exposes friction, not only because a pattern looks cleaner.
3. **Keep presentation separate from rules when practical** — UI should display game state rather than become the source of truth.
4. **Prefer understandable systems over premature complexity**.
5. **Use AI as leverage, not as an authority** — suggestions still require context, review and testing.

## Roadmap

Current priorities:

- [x] Reach a functional MVP
- [x] Validate the main gameplay loop
- [ ] Complete visual-direction rework
- [ ] Standardize UI components and spacing
- [ ] Improve dragon presentation
- [ ] Review technical debt accumulated during MVP development
- [ ] Add public screenshots and GIFs
- [ ] Publish selected technical samples
- [ ] Prepare a distributable demo/build



## Repository policy

The full ARDENS source code and production assets are private.

This repository is intended for:

- Technical portfolio presentation
- Development documentation
- Architecture notes
- Screenshots and demos
- Selected non-sensitive code samples

No production source or third-party licensed assets should be copied here unless they are explicitly safe to redistribute.

## About the developer

ARDENS is developed by **Lucas Queiroz**, Computer Science student and software-development intern working primarily with Java/Spring Boot professionally and C#/Unity in this project.

- GitHub: [Lucas-F-Queiroz](https://github.com/Lucas-F-Queiroz)
- LinkedIn: [lucas-queiroz-54a21b233](https://www.linkedin.com/in/lucas-queiroz-54a21b233/)
