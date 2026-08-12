<div align="center">

# Open Source AI Game Projects

### Start with a working game foundation instead of an empty prompt.

[![Projects](https://img.shields.io/badge/projects-9-7c3aed?style=for-the-badge)](#project-directory)
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
- Lots of others stuff that won't be caught or optimized the first time around

Instead of starting from scratch, begin with an open source project that has already solved many of these expensive problems. The projects below can serve as playable references, reusable foundations, learning resources, or starting points for your own AI-assisted game.

> [!NOTE]
> Project details are summarized from each repository's documentation and manifests. Technologies, features, and licenses can change, so review the source repository before building on it.

## Project directory

Projects are listed alphabetically. Each **last updated** badge reads the latest commit on the project's default branch and refreshes automatically.

| Project | Game / foundation | Primary technologies | License | Activity |
| --- | --- | --- | --- | --- |
| [Blocks Beyond the Stars](#blocks-beyond-the-stars) | 3D voxel space crafting and survival sandbox | Unity, C#, .NET | AGPL-3.0 | [![Last updated](https://img.shields.io/github/last-commit/marceld23/BlocksBeyondTheStars?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/marceld23/BlocksBeyondTheStars/commits/main) |
| [Claude of Duty](#claude-of-duty) | Procedurally generated browser FPS and rendering showcase | JavaScript, Three.js, WebGL2, Web Audio | MIT | [![Last updated](https://img.shields.io/github/last-commit/mshumer/Claude-of-Duty?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/mshumer/Claude-of-Duty/commits/main) |
| [FarmRise Tycoon](#farmrise-tycoon) | Persistent farming and city-building sandbox | TypeScript, Three.js, Next.js, SQLite | Not specified | [![Last updated](https://img.shields.io/github/last-commit/Glitch-Gaming-Platform/Glitch-Games-FarmRise-Tycoon?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/Glitch-Gaming-Platform/Glitch-Games-FarmRise-Tycoon/commits/main) |
| [Glitch Games: Biomes](#glitch-games-biomes) | Restored browser-based multiplayer voxel game foundation | TypeScript, React, Three.js, Node.js | MIT | [![Last updated](https://img.shields.io/github/last-commit/Glitch-Gaming-Platform/Glitch-Games-Biomes?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/Glitch-Gaming-Platform/Glitch-Games-Biomes/commits/main) |
| [Little City](#little-city) | Tiny explorable 3D city planets | JavaScript, Three.js, HTML/CSS | Apache-2.0 | [![Last updated](https://img.shields.io/github/last-commit/craftmygame/little-city?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/craftmygame/little-city/commits/main) |
| [Migla](#migla) | Cozy browser-based skilling MMO | Rust, TypeScript, Three.js, WebSockets | MIT | [![Last updated](https://img.shields.io/github/last-commit/skridlevsky/migla?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/skridlevsky/migla/commits/main) |
| [Monster Breeder](#monster-breeder) | Genetics-driven strategy and simulation game | HTML, JavaScript, Web Workers | GPL-3.0-only | [![Last updated](https://img.shields.io/github/last-commit/jamespetts/MonsterBreeder?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/jamespetts/MonsterBreeder/commits/master) |
| [Regolith](#regolith) | 3D lunar rover survey and exploration game | JavaScript, Three.js, WebGL2, Web Audio | MIT | [![Last updated](https://img.shields.io/github/last-commit/winchxyz/moon-rover?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/winchxyz/moon-rover/commits/main) |
| [World of ClaudeCraft](#world-of-claudecraft) | Full browser MMO with multiplayer and agent training | TypeScript, Three.js, PostgreSQL, Gymnasium | MIT | [![Last updated](https://img.shields.io/github/last-commit/levy-street/world-of-claudecraft?display_timestamp=committer&label=last%20updated&style=flat-square)](https://github.com/levy-street/world-of-claudecraft/commits/main) |

## Blocks Beyond the Stars

**Repository:** [marceld23/BlocksBeyondTheStars](https://github.com/marceld23/BlocksBeyondTheStars)

A block-based 3D space crafting game set across procedurally generated planets and star systems. Players can mine resources, craft equipment, tame creatures, construct bases and space stations, design ships block by block, and play alone or through a self-hosted multiplayer server. The project describes its code, architecture, visual assets, audio, and optional dynamic storytelling systems as AI-created or AI-assisted.

This is a strong starting point for projects that need voxel world generation, crafting, persistence, authoritative multiplayer, vehicles, building systems, or a substantial Unity client/server architecture.

**Technologies:** Unity 6 and URP, C#, .NET 10, ASP.NET Core, SQLite with optional PostgreSQL, LiteNetLib, MessagePack, WebSockets, Docker, and an optional Python FastAPI/LangChain AI service.

**License:** AGPL-3.0

## Claude of Duty

**Repository:** [mshumer/Claude-of-Duty](https://github.com/mshumer/Claude-of-Duty)

A first-person shooter built in the browser by a coordinated fleet of AI agents. Its 11 subsystems cover a procedural urban combat space, first-person movement, weapons and ballistics, enemy perception and cover behavior, custom physics and ragdolls, synthesized spatial audio, and a modern HDR rendering pipeline. Every texture, mesh, animation, and sound is generated from code at load time rather than loaded from external art assets.

This is a strong reference for browser FPS mechanics, procedural asset generation, custom character and projectile physics, enemy combat AI, advanced WebGL rendering, and visual-regression or performance tooling for agent-built games.

**Technologies:** JavaScript ES modules, Three.js r180, WebGL2, Web Audio API, Vite, Playwright, and PNG-based deterministic screenshot comparison tools.

**License:** MIT. The repository's `package.json` currently lists ISC, so downstream users should review the metadata discrepancy before reuse.

## FarmRise Tycoon

**Repository:** [Glitch-Gaming-Platform/Glitch-Games-FarmRise-Tycoon](https://github.com/Glitch-Gaming-Platform/Glitch-Games-FarmRise-Tycoon)

A single-player farming and city-building sandbox with a persistent career. Players plant, tend, harvest, haul, build, trade, specialize, process goods, manage soil and crop quality, hire workers, use finance and insurance systems, respond to disruptive incidents and seasons, expand across multiple parcels, and contribute to town projects. The repository separates its reusable engine, deterministic simulation rules, save migration, UI, generated asset pipeline, and transition-validating backend.

This is a useful foundation for farming or tycoon games that need progression, contracts and markets, deterministic simulation, grid collision and A* pathfinding, persistent saves, mobile controls, generated art and audio pipelines, and extensive automated verification designed for AI-agent contributions.

**Technologies:** TypeScript, Three.js, Vite, Next.js, React, SQLite, Drizzle ORM, Zod, Blender and Python asset tooling, Vitest, Playwright, and Node.js workspaces.

**License:** Not specified. The repository currently has no license file, so review licensing with the maintainers before reusing its code or assets.

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

## Regolith

**Repository:** [winchxyz/moon-rover](https://github.com/winchxyz/moon-rover)

Also titled **Regolith: The Silence at Anaxagoras**, this is a 3D lunar rover survey game that began with a single prompt and was refined through iterative AI-assisted correction rounds. It offers five missions, ground-penetrating radar, core drilling, relay deployment, power and thermal management, a discoverable codex, mobile controls, gamepad support, and an ending-driven exploration campaign on the floor of a lunar crater.

The simulation includes six-wheel suspension, lunar traction and gravity, terrain excavation that feeds back into physics, ballistic dust, procedural terrain and rocks, physically inspired lunar lighting, runtime-generated textures, and synthesized audio. It is a useful starting point for vehicle simulation, deformable terrain, scientific exploration mechanics, procedural audiovisual content, mobile WebGL, or compact no-build browser games.

**Technologies:** JavaScript ES modules, vendored Three.js r160, WebGL2, Web Audio API, HTML, CSS, import maps, `localStorage`, and a dependency-free Node.js static server. The game has no build step or downloaded runtime assets.

**License:** MIT

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
