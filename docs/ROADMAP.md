# ARDENS Roadmap

ARDENS is a private Unity production project presented publicly through this repository. The roadmap below describes the direction without exposing production source or licensed assets.

## Current position

- Functional MVP baseline completed.
- Core gameplay loop validated in Unity.
- Visual and UX rework in progress.
- Public showcase reorganized around real screenshots, animation frames and a short walking GIF.

## Next product and engineering steps

1. Continue the visual rework with consistent pixel-art scale, hierarchy and UI spacing.
2. Add more real player evidence as the build evolves.
3. Publish carefully selected, portfolio-safe technical examples.
4. Prepare a distributable demo when the presentation layer is stable.

## Machine learning: DragonLab

Machine learning is planned as a balance-testing laboratory, not as a feature that controls the player-facing game.

DragonLab will eventually:

- run headless simulations using the same economy and progression rules as the game;
- compare aggressive, conservative, casual, greedy and random agent profiles;
- record milestones, idle windows, return on investment and dominant strategies;
- compare balance changes before and after a definition or price update;
- generate evidence for human review instead of changing the game automatically.

The implementation order is deliberate:

1. deterministic simulation environment;
2. random and heuristic baselines;
3. versioned telemetry and regression reports;
4. trainable ML policies;
5. Codex-assisted analysis with human approval before any design change.

DragonLab is currently a roadmap item. No ML capability is claimed as already implemented in the player.
