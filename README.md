# 🎮 Game Development Portfolio — Brad Barroso

**Multi-engine game developer** specializing in AI-driven game systems, procedural content generation, and building intelligent digital assets for research and production environments.

---

## 🔧 Engine Proficiency

| Engine | Language | Project | Focus Area |
|--------|----------|---------|------------|
| **Godot 4** | GDScript / C# | [Procedural AI Dungeon](https://github.com/bradleybeatz1313/godot-procedural-ai) | Procedural generation + A* pathfinding + AI director |
| **Defold** | Lua | [AI Behavior Tree System](https://github.com/bradleybeatz1313/defold-behavior-trees) | Modular behavior trees + finite state machines |
| **Solar2D** | Lua | [Neural Agent Simulation](https://github.com/bradleybeatz1313/solar2d-neural-agents) | Neural network-driven autonomous agents |
| **Panda3D** | Python | [RL Training Environment](https://github.com/bradleybeatz1313/panda3d-rl-environment) | Reinforcement learning gym for 3D navigation |
| **Stride (Xenko)** | C# | [Procedural Terrain + ML Nav](https://github.com/bradleybeatz1313/stride-procedural-terrain) | Procedural terrain generation + ML-based navigation |

---

## 🧠 Core Competencies

### AI & Game Systems
- **Behavior Trees & FSMs** — Designed and implemented modular AI decision-making frameworks across multiple engines
- **Procedural Content Generation** — Dungeon generation (BSP, cellular automata, wave function collapse), terrain (noise-based, erosion simulation), asset placement
- **Pathfinding** — A*, navigation meshes, flow fields, hierarchical pathfinding
- **Reinforcement Learning Integration** — OpenAI Gym-compatible training environments built inside game engines
- **AI Directors** — Dynamic difficulty adjustment and pacing systems

### Technical
- **Languages:** GDScript, Lua, Python, C#, C++, JavaScript/TypeScript
- **3D Pipelines:** Modeling, rigging, shader authoring (GLSL/HLSL), PBR workflows
- **Tooling:** Git, CI/CD, automated testing for game systems, profiling & optimization
- **Prior Engine Experience:** Unreal Engine 5 (Blueprints + C++), Unity

---

## 📐 Architecture Philosophy

Every project in this portfolio follows the same principles:

1. **Separation of concerns** — Game logic, AI systems, and rendering are decoupled
2. **Data-driven design** — Behaviors, level parameters, and agent configs are externalized to JSON/Resources
3. **Testability** — AI systems include standalone test harnesses and visualization tools
4. **Documentation** — Every module has inline docs, architecture diagrams, and setup instructions

---

## 🔬 AI Research Relevance

These projects are specifically designed to demonstrate capabilities relevant to AI research in game environments:

- **Digital asset generation** — Procedural systems that create game-ready assets programmatically
- **Agent environments** — Game worlds purpose-built as training grounds for AI agents
- **Evaluation frameworks** — Built-in metrics, logging, and visualization for AI behavior analysis
- **Cross-engine portability** — Proven ability to implement equivalent systems across different engines and paradigms

---

## 📬 Contact

- **GitHub:** [bradleybeatz1313](https://github.com/bradleybeatz1313)
- **Email:** bradley.s.barroso@gmail.com
- **LinkedIn:** [Brad Barroso](https://www.linkedin.com/in/bradley-barroso-aa64ba372)

---

*Each project includes full source code, setup instructions, architecture documentation, and demo recordings.*

---

## Quick Start

Clone any individual project:

    git clone https://github.com/bradleybeatz1313/godot-procedural-ai

For the Python RL environment:

    pip install -r requirements.txt
    python training/train.py

---

## Tools and Dependencies

| Project | Runtime | Key Libraries |
|---------|---------|---------------|
| Godot Procedural AI | Godot 4.3+ | GDScript, AStar2D |
| Defold Behavior Trees | Defold 1.6+ | Lua 5.1 |
| Solar2D Neural Agents | Solar2D 2024.x | Lua 5.1 |
| Panda3D RL Environment | Python 3.10+ | Gymnasium, SB3 |
| Stride Procedural Terrain | .NET 6+ | Stride 4.1 |

---

## Testing Philosophy

Every AI system ships with a standalone test harness:

- **Godot / Defold**: Scene-level debug visualizations (perception cones, path overlays, BT state)
- **Panda3D**: Headless pytest suite covering env reset, step, reward shaping, and edge cases
- **Stride**: Unit tests for noise generation, biome classification, and mesh normal accuracy

---

## System Requirements

| Engine | Min Version | Notes |
|--------|------------|-------|
| Godot | 4.2 | Requires NavigationServer2D |
| Defold | 1.6.0 | Socket library for BT cooldown timing |
| Solar2D | 2024.3757 | physics.newBody required |
| Panda3D | 1.10.13 | Python 3.10+ recommended |
| Stride | 4.1 | .NET 6 SDK required |

---

## Architecture Highlights

**Godot Procedural AI**: BSP dungeon generation, hierarchical A*, priority-selector BT with 5 behavior layers.

**Defold Behavior Trees**: Zero-allocation tree construction via table pooling, composable decorators with resumable state.

**Panda3D RL Environment**: Gymnasium-compatible with full SB3/CleanRL support. 24-dim observation: lidar + velocity + heading + target.

**Solar2D Neural Agents**: Neuroevolution via genetic algorithms -- no backprop. Xavier init, crossover, Gaussian mutation.

**Stride Terrain**: Streaming LOD terrain with biome classification and ML-based navigation agent.

---

## Research Applications

- **Reproducibility**: Seeded RNG throughout -- every run is deterministic when seeded
- **Observability**: Per-step info dicts, event buses, and debug draw layers
- **Extensibility**: All agent configs are data-driven (JSON/Resources), not hard-coded
- **Benchmarking**: Built-in episode metrics logged for offline analysis

---

## Project Status

| Repository | Status | Last Updated |
|-----------|--------|-------------|
| godot-procedural-ai | Active | 2025-08 |
| defold-behavior-trees | Active | 2025-08 |
| solar2d-neural-agents | Active | 2025-08 |
| panda3d-rl-environment | Active | 2025-07 |
| stride-procedural-terrain | Active | 2025-07 |

---

## Engine Philosophy

- **Godot 4**: Best-in-class GDScript tooling, native NavigationServer, fully open source
- **Defold**: Extremely lightweight runtime; ideal for demonstrating pure logic with zero overhead
- **Solar2D**: Proven mobile physics; tests neural evolution under real 2D constraints
- **Panda3D**: Python-native; bridges game engine and ML library ecosystems
- **Stride**: Full .NET 6 stack; demonstrates enterprise C# game development practices

---

## Roadmap

- [ ] Unity project demonstrating DOTS-based AI (ECS behavior trees)
- [ ] Unreal Engine 5 project with Mass Entity + StateTree
- [ ] Shared benchmark suite comparing agent performance across engines
- [ ] Docker-based headless training environment for Panda3D

---

## Key Design Patterns

All projects follow the same structural patterns:

1. **Event Bus**: Decoupled agent-to-world communication; no direct node references
2. **Config Resources**: Agent stats, tree parameters, and env configs are externalized
3. **Blackboard**: Shared read/write context passed through every AI decision
4. **Component Composition**: Perception, steering, and decision are separate, swappable systems
