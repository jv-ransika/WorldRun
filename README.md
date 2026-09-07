# WorldRun

**WorldRun** is an open-source project for building programmable simulated worlds where different decision-making systems can observe the world, take actions, and change what happens over time.

![[overview_architecture.png]]

---

## 🌍 Ultimate Goal

The long-term goal of WorldRun is to become a **general-purpose simulation runtime**.

Developers should eventually be able to define worlds containing:

* entities
* resources
* actions
* events
* rules
* constraints
* failures
* time
* metrics

Different decision-makers could then interact with those worlds:

* rule-based algorithms
* optimization algorithms
* reinforcement learning agents
* LLM agents
* human controllers

The idea is simple:

> **Build a world. Give something a goal. Let it act. See what happens.**
---

## 🚀 Immediate Goal

### Milestone 1 — Make the World Alive

We are **not building the complete WorldRun vision yet**.

The first goal is intentionally small:

> Build a tiny visual 2D space-station simulation and establish the basic foundation of the runtime.

For this milestone, the world only needs to support:

* simulation time
* basic entities
* 2D positions
* entity movement
* simple resources
* live world-state updates
* a basic browser visualization

The current objective is simply:

> **Create a small world that is alive, visible, and built on a clean foundation we can extend later.**

---

# 🛠 Initial Tech Stack

* **Python** — simulation core
* **FastAPI** — backend/API
* **WebSocket** — live world updates
* **React + TypeScript** — frontend
* **Phaser.js** — 2D visualization
* **Pytest** — testing

---

# 🤝 Contributing

WorldRun is being built incrementally.

Each milestone will be divided into small GitHub issues so contributors can work on individual parts without needing to understand the entire project.

The current focus is:

> **Milestone 1 — Make the World Alive**

Check the GitHub Issues page for available tasks.
