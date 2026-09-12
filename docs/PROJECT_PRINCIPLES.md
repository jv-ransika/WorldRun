# Project Principles

These principles are intended to keep WorldRun focused as the project grows.

## Core Principles

1. **Useful without AI**
   - WorldRun should remain useful even when no AI component is used.
   - AI-based decision-makers are optional, not required.

2. **Decision-makers do not directly modify world state**
   - Decision-makers should propose actions.
   - The simulation runtime should validate and apply state changes.

3. **Simulation core is independent from visualization**
   - The simulation should run without any renderer or UI.
   - Visualization layers should consume simulation outputs without owning simulation logic.

4. **Runtime stays domain-independent**
   - The core runtime should support many domains, not only one scenario.
   - Domain rules should be implemented as world-specific modules on top of the runtime.

5. **Prefer simple solutions**
   - Use the simplest design that solves the current problem.
   - Avoid adding complexity before it is clearly needed.

6. **Each milestone must produce visible or useful output**
   - Every milestone should result in something demonstrable, testable, or practically usable.
   - Progress should be concrete, not only architectural planning.

7. **Prioritize reproducibility and determinism**
   - Simulations should be reproducible when inputs and seeds are the same.
   - Deterministic behavior should be a default goal, especially for testing and debugging.

8. **Add abstractions only for real needs**
   - Introduce new abstractions only when repeated use-cases or clear pain points justify them.
   - Do not generalize early without evidence.

## Current Non-Goals

- WorldRun is **not** a game engine.
- WorldRun is **not** an LLM framework.
- WorldRun is **not** a full physics engine.
- WorldRun is **not** intended to replace SimPy, Mesa, PettingZoo, or similar projects.

