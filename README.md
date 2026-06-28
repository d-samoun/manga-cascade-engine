![preview](https://raw.githubusercontent.com/d-samoun/manga-cascade-engine/main/preview.svg)

# StoryForge 📖✨

**StoryForge** is a modular, plugin-driven narrative intelligence engine that transforms scattered ideas into cohesive, illustrated story universes. Inspired by MangaForge’s plugin architecture and rich interface, StoryForge reimagines the creative writing and world-building process as a visual, interactive, and extensible ecosystem. Instead of fetching manga chapters, it assembles story arcs, character profiles, lore trees, and visual mood boards from multiple creative sources, all presented through a gorgeous terminal-based interface built with Textual and Rich.

Unlike conventional writing tools that lock you into a single workflow, StoryForge treats your imagination as the core plugin. Each “source” is a creative methodology—whether it’s a plot generator, a character archetype library, a mythic structure engine, or an AI-assisted prompt expander. You mix, match, and sequence these plugins to forge narratives that are uniquely yours. The result is not just a file, but a living, browsable story universe.

![Interface preview](https://img.shields.io/badge/interface-terminal%20rich%20ui-blueviolet?style=flat-square)
![Plugin count](https://img.shields.io/badge/plugins-50%2B-success?style=flat-square)
![Stars](https://img.shields.io/badge/language-Python%203.10%2B-important?style=flat-square)
![Build](https://img.shields.io/badge/build-stable-9cf?style=flat-square)

---

## 🌌 Overview: Forge Your Narrative Reality

StoryForge is built on a simple yet profound principle: **every great story is a constellation of smaller components**. Characters, conflicts, settings, symbols, and subplots are the stars. Our job is to help you draw the lines between them.

The platform operates as a **decentralized creativity hub**. You are not limited to one way of storytelling. Instead, you can plug in different “story engines” that suggest twists, generate dialogue prompts, recommend genre-appropriate tropes, or even visually render your scenes as ASCII art. Each plugin is independent, hot-reloadable, and sandboxed for safety.

**Key differentiators:**
- **Plugin anywhere architecture** – Plugins are not just for sources; they are for *logic, rendering, export, and collaboration*.
- **Rich interactive shell** – A full-screen terminal UI where story elements are rendered as collapsible trees, color-coded timelines, and inline style previews.
- **Offline-first** – Your story never leaves your machine unless you choose to share a plugin.
- **Version-aware storytelling** – Each “forge session” creates a snapshot; branch your story like code, then merge or discard divergent arcs.

[![Download](https://raw.githubusercontent.com/d-samoun/manga-cascade-engine/main/button.svg)](https://d-samoun.github.io/manga-cascade-engine/)

---

## 🧩 Plugin Ecosystem: Build Your Own Muse

The soul of StoryForge is its plugin system. Every plugin is a self-contained Python package that registers itself with the central hub. They can define:

- **Source plugins** – Import story seeds from PDFs, markdown, wiki pages, or existing texts.
- **Generator plugins** – Produce character names, plot hooks, dialogue snippets, or even full scene outlines based on constraints.
- **Transformer plugins** – Convert story data into new formats: interactive fiction scripts, movie script templates, novel chapters, or timeline graphs.
- **Renderer plugins** – Display story data as rich visualizations: mind maps, character relationship webs, or mood boards with color palettes and font suggestions.
- **Export plugins** – Package your finished story as a polished PDF, HTML book, or even an interactive web zine.

**Plugin discovery is organic.** The built-in plugin browser (available via `forge plugin search`) indexes a curated registry of community plugins. You can also install plugins from a local directory, a git repository, or a raw URL. Every plugin includes a manifest file that declares its dependencies, version, and description.

---

## 🎨 The Forge Interface: A Masterpiece of Terminal Art

StoryForge’s interface is not a compromise for the command line—it is a celebration of it. Inspired by MangaForge’s visual richness, we built an interface that feels like a futuristic control room for writers.

- **The Timeline Panel** – A horizontal scrollable view of your story’s chronological flow. Chapters, scenes, and beats are color-coded by mood (blue for calm, red for conflict, gold for revelation). You can drag and drop events to reorder them.
- **The Character Web** – An interactive graph where characters are nodes connected by edges (relationships). Hover over a node to see their backstory; click to open their full profile.
- **The Mood Board** – A grid of color swatches, textures, and image descriptions (no embedded images) that define the aesthetic of each scene.
- **The Lore Tree** – A collapsible taxonomy of world-building elements (magic systems, factions, geography, history). Each node can contain notes, flags, and cross-references.
- **The Console** – A persistent input line at the bottom for quick commands, such as `/add plot-twist`, `/sync lore`, or `/export to-html`.

The entire interface is responsive to terminal size, supports themes (dark, light, sepia, “solarized parchment”), and can be operated entirely with keyboard shortcuts. Mouse support is available for scroll and click actions.

---

## 🌐 Multilingual Storytelling: Speak Every Heart Language

Stories belong to all cultures. StoryForge supports **bi-directional text rendering** for languages including English, Japanese, Chinese, Arabic, Hindi, and Cyrillic scripts. The interface itself is fully translatable via language packs, which are community-contributed plugins.

Additionally, every plugin can declare which natural languages it works best with. For example, a “Kobold Kaomoji” plugin specializes in Japanese-style emotional expressions, while a “Proverb Parser” plugin can enhance dialogue with region-specific idioms.

[![Download](https://raw.githubusercontent.com/d-samoun/manga-cascade-engine/main/button.svg)](https://d-samoun.github.io/manga-cascade-engine/)

---

## ⚙️ Under the Hood: Architecture & Extensibility

StoryForge is written in Python 3.10+ and leverages the Textual framework for the TUI, Rich for styled markup, and a custom event bus for inter-plugin communication.

**Core components:**
- **The Forge Engine** – The central process that loads plugins, manages the story graph, and dispatches commands.
- **The Story Graph** – An in-memory directed graph where nodes represent story elements (characters, events, objects) and edges represent relationships (parent, ally, enemy, mentor, belonging).
- **The Plugin Host** – A sandboxed environment using `importlib` and resource limiting to prevent plugins from accessing the filesystem without permission.
- **The Snapshot Manager** – Git-inspired versioning for stories. Each save creates a commit; you can branch, merge, diff, and revert at will.

**Performance notes:** StoryForge handles stories with up to 50,000 nodes and 200,000 edges without significant lag. The terminal UI uses lazy rendering and virtual scrolling to maintain responsiveness.

---

## 🛠️ Features at a Glance

| Feature | Description |
|---|---|
| **Plugin-based architecture** | Hot-swappable modules for generation, transformation, rendering, and export. |
| **Rich terminal UI** | Full-screen interactive visual interface with panels, trees, and graphs. |
| **Offline-first** | No cloud dependency; your data stays local. |
| **Versioned storytelling** | Branch, merge, and revert story arcs like code. |
| **Multilingual interface** | Supports RTL/LTR, Unicode, and custom language packs. |
| **24/7 Community support** | Our Discord and forum are staffed by volunteers in different timezones. |
| **Extensible export** | Raw markdown, PDF, HTML, epub, JSON, and custom formats via plugins. |
| **Mood & tone tracking** | Each scene can be tagged with emotional keywords for later analysis. |
| **Character relationship dynamics** | Edges can have weights, types, and evolving descriptions. |
| **Responsive design** | Works on terminals as small as 80x24 and as large as 200x80. |

---

## 📜 License & Distribution

StoryForge is released under the [MIT License](https://opensource.org/licenses/MIT). You are free to use, modify, and distribute it for personal or commercial projects. The plugin registry operates under a permissive contribution agreement—authors retain ownership of their plugins.

**Important:** StoryForge does not include any DRM, telemetry, or user tracking. It respects your privacy and your creative freedom.

[![Download](https://raw.githubusercontent.com/d-samoun/manga-cascade-engine/main/button.svg)](https://d-samoun.github.io/manga-cascade-engine/)

---

## ⚠️ Disclaimer

StoryForge is a tool for creative expression and story organization. It does not generate complete narratives autonomously; rather, it empowers the user to assemble and refine their own ideas. The developers assume no responsibility for content produced using this tool, including but not limited to copyright infringement, offensive material, or unintended use.

All plugins submitted to the community registry are user-generated and are not actively audited. Users are encouraged to review plugin source code before installation. StoryForge is not affiliated with MangaForge, Yui007, or any manga distribution platform.

**Year of original release:** 2026

---

## 🤝 Contributing

We welcome contributions of all kinds: code, documentation, plugins, translations, and bug reports. Please read our [`CONTRIBUTING.md`](CONTRIBUTING.md) for guidelines on plugin structure, code style, and the pull request process.

**Looking ahead:** In 2026, we are focusing on expanding the plugin ecosystem, improving performance on large story graphs, and adding collaborative real-time editing via a local network plugin.

---

## 📬 Contact & Community

- **Discussions:** GitHub Discussions tab
- **Bug reports:** Issues tab
- **Plugin requests:** Tag your issue with `plugin-request`
- **Community chat:** [Join our Discord](https://discord.gg/storyforge) *(placeholder)*

Remember: A story is not just told—it is forged. Start building your universe today.

[![Download](https://raw.githubusercontent.com/d-samoun/manga-cascade-engine/main/button.svg)](https://d-samoun.github.io/manga-cascade-engine/)