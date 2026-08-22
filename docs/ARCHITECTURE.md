# ARDENS Architecture

This document describes ARDENS at a portfolio-safe level. The production source code remains private.

## Goals

The architecture is intended to support a game that can continue evolving after the MVP without forcing every new feature into a single tightly coupled flow.

The current priorities are:

- Clear ownership of game state
- Separation between gameplay rules and presentation
- Reusable UI patterns
- Systems that can be refactored independently
- Persistence that does not depend on scene-only state
- Low friction when adding or changing progression content

## High-level areas

### Gameplay

Contains rules and state transitions related to progression, economy, inventory, dragons and player actions.

### Presentation

Responsible for rendering information and collecting user input. UI components should avoid becoming the authoritative source of gameplay state.

### Data

Represents runtime state, configuration and persistent information.

### Infrastructure

Shared concerns such as save/load, services, integration points and development tooling.

## Why this structure matters

The first MVP prioritized proving the game loop. Once the loop worked, the project moved into a stage where duplicated logic, inconsistent presentation and tightly connected behaviors became easier to identify.

The current refactoring effort is therefore evidence-driven: systems are reorganized based on friction found while actually developing and using the MVP.

## Public documentation policy

This repository intentionally avoids publishing:

- Full production source
- Proprietary game assets
- Third-party licensed packages
- Credentials or private service configuration

Selected code samples may be added only when they are isolated, understandable and safe to redistribute.
