<div align="center">

# Open Source AI Game Projects

### Start with a working game foundation instead of an empty prompt.

[![Projects](https://img.shields.io/badge/projects-6-7c3aed?style=for-the-badge)](#project-directory)
[![Pull requests welcome](https://img.shields.io/badge/pull_requests-welcome-22c55e?style=for-the-badge)](#add-a-project)

</div>

One prompt can make a game look nearly finished. The hard truth is that the first playable scene is usually the beginning, not the end. Shipping a complete game can consume hundreds of hours—or a large number of AI tokens—because every additional system creates more design, implementation, integration, balancing, and testing work.

That work often includes:

- NPC interactions and enemy AI
- Combat systems and character controls
- Animation and physics systems
- Rendering pipelines, GPU/CPU load, and frame-rate optimization
- Quest, progression, inventory, and economy systems
- Multiplayer networking and server authority
- Mobile controls and performance optimization
- Automated testing and reproducible simulation
- Content pipelines and large-scale game balancing

Instead of starting from scratch, begin with an open source project that has already solved many of these expensive problems. The projects below can serve as playable references, reusable foundations, learning resources, or starting points for your own AI-assisted game.

> [!NOTE]
> Project details are summarized from each repository's documentation and manifests. Technologies, features, and licenses can change, so review the source repository before building on it.

## Project directory

Projects are listed alphabetically. Each **last updated** badge reads the latest commit on the project's default branch and refreshes automatically.

| Project | Game / foundation | Primary technologies | License | Activity |
| --- | --- | --- | --- | --- |
| [Blocks Beyond the Stars](#blocks-beyond-the-stars) | 3D voxel space crafting and survival sandbox | Unity, C#, .NET | AGPL-3.0 | [![Last updated](https://img.shields.io/github/last-commit/marceld23/BlocksBeyondTheStars?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/marceld23/BlocksBeyondTheStars/commits/main) |
| [Glitch Games: Biomes](#glitch-games-biomes) | Restored browser-based multiplayer voxel game foundation | TypeScript, React, Three.js, Node.js | MIT | [![Last updated](https://img.shields.io/github/last-commit/Glitch-Gaming-Platform/Glitch-Games-Biomes?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/Glitch-Gaming-Platform/Glitch-Games-Biomes/commits/main) |
| [Little City](#little-city) | Tiny explorable 3D city planets | JavaScript, Three.js, HTML/CSS | Apache-2.0 | [![Last updated](https://img.shields.io/github/last-commit/craftmygame/little-city?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/craftmygame/little-city/commits/main) |
| [Migla](#migla) | Cozy browser-based skilling MMO | Rust, TypeScript, Three.js, WebSockets | MIT | [![Last updated](https://img.shields.io/github/last-commit/skridlevsky/migla?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/skridlevsky/migla/commits/main) |
| [Monster Breeder](#monster-breeder) | Genetics-driven strategy and simulation game | HTML, JavaScript, Web Workers | GPL-3.0-only | [![Last updated](https://img.shields.io/github/last-commit/jamespetts/MonsterBreeder?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/jamespetts/MonsterBreeder/commits/master) |
| [World of ClaudeCraft](#world-of-claudecraft) | Full browser MMO with multiplayer and agent training | TypeScript, Three.js, PostgreSQL, Gymnasium | MIT | [![Last updated](https://img.shields.io/github/last-commit/levy-street/world-of-claudecraft?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/levy-street/world-of-claudecraft/commits/main) |

## Blocks Beyond the Stars

**Repository:** [marceld23/BlocksBeyondTheStars](https://github.com/marceld23/BlocksBeyondTheStars)

A block-based 3D space crafting game set across procedurally generated planets and star systems. Players can mine resources, craft equipment, tame creatures, construct bases and space stations, design ships block by block, and play alone or through a self-hosted multiplayer server. The project describes its code, architecture, visual assets, audio, and optional dynamic storytelling systems as AI-created or AI-assisted.

This is a strong starting point for projects that need voxel world generation, crafting, persistence, authoritative multiplayer, vehicles, building systems, or a substantial Unity client/server architecture.

**Technologies:** Unity 6 and URP, C#, .NET 10, ASP.NET Core, SQLite with optional PostgreSQL, LiteNetLib, MessagePack, WebSockets, Docker, and an optional Python FastAPI/LangChain AI service.

**License:** AGPL-3.0

## Glitch Games: Biomes

**Repository:** [Glitch-Gaming-Platform/Glitch-Games-Biomes](https://github.com/Glitch-Gaming-Platform/Glitch-Games-Biomes)

A Glitch-maintained restoration of the open source Biomes codebase. The fork reconstructs the local asset snapshot workflow after the original public snapshot endpoint went offline, making the large browser-based voxel game codebase usable again for local development, research, experimentation, and new game projects.

This is a useful foundation for multiplayer voxel worlds, entity-component systems, server-authoritative gameplay, browser rendering, procedural asset pipelines, NPC systems, and large-scale online game architecture.

**Technologies:** TypeScript, React, Next.js, Three.js, Node.js, WebSockets, Redis, Bazel, Python asset tooling, Rust/C++/WebAssembly components, Docker, and Kubernetes deployment tooling.

**License:** MIT

## Little City

**Repository:** [craftmygame/little-city](https://github.com/craftmygame/little-city)

A collection of tiny, explorable city planets built for the browser. Little Taipei presents landmarks, roads, parks, shops, and transit around a cel-shaded globe using real relative bearings and distances; the repository also contains work for Little Paris and is designed to grow into more cities. Its small, focused landmark files are intentionally friendly to contributions made with coding agents.

This is a good starting point for stylized city exploration, procedural buildings, geographic placement, lightweight character movement, browser-based 3D scenes, and agent-friendly content contribution workflows.

**Technologies:** JavaScript ES modules, Three.js, HTML, CSS, Node.js validation scripts, Python's static HTTP server for local development, and optional Antics multiplayer deployment.

**License:** Apache-2.0

## Migla

**Repository:** [skridlevsky/migla](https://github.com/skridlevsky/migla)

A small, cozy skilling MMO that runs in the browser. Players gather resources, fish, cook, contribute to a shared town fire, and fight old machines beyond the town. The project was developed primarily by AI agents under human direction and includes a deterministic simulation, authoritative server, shared protocol, persistence, load-testing bots, and a hand-authored world.

This is an excellent reference for deterministic multiplayer simulation, shared-world skilling systems, authoritative WebSocket networking, headless bots, soak testing, and keeping a browser client synchronized with a Rust server.

**Technologies:** Rust, TypeScript, Three.js, Vite, WebSockets, JSON wire messages, Cargo, and Vitest.

**License:** MIT

## Monster Breeder

**Repository:** [jamespetts/MonsterBreeder](https://github.com/jamespetts/MonsterBreeder)

A browser-based strategy and simulation game about breeding a genetically evolving population of autonomous monsters to defend treasure from adventurers. Seasonal management alternates with real-time raids across procedurally generated terrain, while inheritance, mutation, selection, injuries, disease, nutrition, ageing, pathfinding, morale, and environmental pressure shape the population over time.

This is a useful starting point for genetics simulations, autonomous agents, procedural terrain, emergent behavior, simulation-heavy strategy games, save migration, and complex systems that run without a build step.

**Technologies:** A self-contained HTML/CSS/JavaScript game, browser Web Workers for the authoritative simulation, browser local storage, JSON import/export, and Python test/tutorial harnesses.

**License:** GPL-3.0-only

## World of ClaudeCraft

**Repository:** [levy-street/world-of-claudecraft](https://github.com/levy-street/world-of-claudecraft)

A complete classic-era MMO that runs in the browser and can also be self-hosted. It includes classes and talent trees, quests, open-world zones, dungeons and raids, PvP, professions, a player economy, guilds, trading, achievements, mobile and desktop clients, server-authoritative multiplayer, and a headless reinforcement-learning environment that uses the same deterministic game core.

This is one of the broadest foundations in the directory for studying how combat, progression, quests, multiplayer persistence, instancing, economies, performance scaling, native packaging, and AI-agent training fit together in a large game.

**Technologies:** TypeScript, Three.js, Vite, Vitest, Node.js, WebSockets, PostgreSQL, Docker, Electron, Capacitor, Python, and Gymnasium.

**License:** MIT

## Automatic last-updated badges

The activity badges use the Shields.io `github/last-commit` endpoint. They are rendered when this README is viewed and update from the source repository automatically, subject to normal GitHub and badge caching. No scheduled GitHub Action is required.

Use this pattern when adding another project:

```md
[![Last updated](https://img.shields.io/github/last-commit/OWNER/REPOSITORY?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/OWNER/REPOSITORY/commits/BRANCH)
```

## Add a project

Pull requests are welcome. Please add projects that are open source, meaningfully built with or for AI-assisted development, and substantial enough to provide reusable game systems or a useful starting point.

When adding a project:

1. Place it in alphabetical order in both the directory table and the detailed list.
2. Link directly to the source repository.
3. Explain what the game is and why it is a useful foundation.
4. List the primary technologies and license.
5. Include a live last-updated badge.
6. Keep descriptions factual and based on the project's current documentation.

If your project belongs here, open a pull request and tell us what makes it useful to other AI game builders.
