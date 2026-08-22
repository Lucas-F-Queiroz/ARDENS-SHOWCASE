# AI-assisted development workflow

ARDENS uses AI as part of the software-development process, with OpenAI Codex being the primary tool.

The objective is not to delegate technical ownership. The objective is to reduce the cost of investigation, iteration and review while keeping decisions grounded in the actual project.

The next planned engineering laboratory is **DragonLab**: a headless simulation environment that will use the game's rules to test balance with reproducible agents and telemetry. It is a development tool, not an AI dependency inside the player.

## Typical workflow

### 1. Inspect before changing

Before a larger change, the relevant code and project context are inspected first.

AI is used to help:

- Map dependencies
- Locate repeated responsibilities
- Identify files affected by a change
- Summarize unfamiliar parts of the codebase

### 2. Plan the change

For changes that touch multiple systems, I prefer producing a concrete implementation plan before editing.

The plan normally defines:

- Scope
- Files/systems affected
- Expected behavior
- Constraints
- Validation steps
- What should explicitly not change

### 3. Implement incrementally

Changes are applied in small enough steps to keep failures understandable.

AI may generate or modify code, but the result is checked against:

- Existing architecture
- Unity behavior
- Project conventions
- Intended gameplay
- Side effects on adjacent systems

### 4. Validate

Validation can include:

- Running the project in Unity
- Checking the affected UI/gameplay flow
- Reviewing diffs
- Searching for duplicated or dead code
- Verifying that unrelated behavior did not change

### 5. Refactor and document

After functionality works, AI is also used to:

- Reduce duplication
- Improve naming
- Reorganize responsibilities
- Update documentation
- Record decisions for future iterations

## Visual-development use

During the current visual rework, AI is also used to help define a consistent art direction and to structure prompts for external visual tooling.

The important constraint is consistency: generated assets are evaluated against the project's visual rules rather than accepted as isolated outputs.

## What I avoid

- Blindly accepting large generated patches
- Adding abstraction only because it looks architecturally sophisticated
- Treating generated code as automatically correct
- Letting AI redefine product scope without review
- Publishing internal or licensed material through prompts or public repositories

## Why document this

AI-assisted development is increasingly part of real engineering workflows. The interesting skill is not simply knowing how to prompt a model; it is using the tool while retaining context, judgment, validation and responsibility for the final system.
