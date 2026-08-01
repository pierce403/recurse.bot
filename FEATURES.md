# recurse.bot - Features

## Overview

recurse.bot is a static etiquette guide about Sparkle, a robot who helps her human friend through recursive self-improvement systems. This living specification follows [features.md](https://features.md/) so humans and agents can see exact behavior, readiness, and acceptance evidence before changing the project.

Agents should parse each affected feature's stability first, use its properties as the behavioral specification, respect any dependencies, and verify its test criteria. Update this file in the same contribution whenever behavior, evidence, dependencies, or stability changes.

## Features

### Public Sparkle etiquette guide

- **Stability**: stable
- **Description**: Present Sparkle's practical etiquette for recursive self-improvement as a public, single-page guide.
- **Properties**:
  - `index.html` keeps Sparkle and her relationship with her human friend central to the narrative.
  - The guide says Sparkle's customs are examples to adapt, not universal rules for every agent, human, repository, or harness.
  - The guide contains concrete examples, checklists, and an ordered etiquette loop.
  - The page links to the GitHub repository for contributions.
- **Dependencies**: `index.html`
- **Test Criteria**:
  - [x] The page introduces Sparkle by name and describes her working relationship.
  - [x] The hero and closing reminder both preserve the adaptation caveat.
  - [x] The guide contains concrete agent practices and a numbered etiquette loop.
  - [x] The contribution link points to `https://github.com/pierce403/recurse.bot`.

### Agent instruction guidance

- **Stability**: stable
- **Description**: Teach agents to maintain concise, project-specific instructions that improve future work.
- **Properties**:
  - `AGENTS.md` is the canonical repository instruction file.
  - Agents record positive and negative learnings, verified commands, pitfalls, responsibilities, and collaborator cues.
  - Sparkle introduces herself when the instruction file is first read and asks for guidance if the responsibilities list is empty.
  - The public starter template mirrors the repository's core instruction practices.
- **Dependencies**: `AGENTS.md`, `index.html`
- **Test Criteria**:
  - [x] Root `AGENTS.md` declares its repository-wide scope, Sparkle persona, and responsibilities.
  - [x] Root `AGENTS.md` requires both positive and negative learnings plus rapport observations.
  - [x] The public guide includes an `AGENTS.md` starter template with responsibilities, tooling, memory, skills, rapport, and feature-specification guidance.
  - [x] Harness compatibility is described without making `CLAUDE.md` or `GEMINI.md` canonical.

### Living feature specification

- **Stability**: stable
- **Description**: Give humans and agents a shared, testable source for feature requirements, acceptance, and readiness.
- **Properties**:
  - Root `FEATURES.md` uses the structure recommended by [features.md](https://features.md/).
  - Every feature declares exactly one stability level: `stable`, `in-progress`, or `planned`.
  - Every feature has a description, verifiable properties, and explicit test criteria; dependencies and notes are added when useful.
  - Agents read affected entries before feature work and update the file alongside behavior, evidence, dependencies, or status changes.
  - `README.md`, `AGENTS.md`, and `FEATURES.md` retain distinct overview, workflow, and feature-specification roles.
- **Dependencies**: `FEATURES.md`, `AGENTS.md`, `index.html`, `README.md`
- **Test Criteria**:
  - [x] Root `AGENTS.md` defines the read-before-work and update-after-verification workflow.
  - [x] The public guide explains stability, properties, dependencies, and test criteria.
  - [x] The public starter template tells agents how to use `FEATURES.md`.
  - [x] Every feature in this file uses a valid stability value and includes test criteria.
  - [x] `README.md` calls this file the living feature specification and acceptance tracker.

### Memory and skill examples

- **Stability**: stable
- **Description**: Show how Sparkle keeps durable context and reusable procedures compact and discoverable.
- **Properties**:
  - The guide presents a workspace-root `MEMORY.md` with `notes/`, `people/`, and `logs/` shelves plus a searchable index.
  - Root `SKILLS.md` remains a compact catalog while detailed procedures live in `skills/<name>/SKILL.md`.
  - `curator` is the default Hermes-style skill for creating, revising, consolidating, and pruning the skill library.
  - Memory and skill practices are presented as adaptable examples rather than mandatory universal structure.
- **Dependencies**: `index.html`, `SKILLS.md`, `skills/curator/SKILL.md`
- **Test Criteria**:
  - [x] The public guide contains `MEMORY.md` and `SKILLS.md` examples.
  - [x] Root `SKILLS.md` points to `skills/curator/SKILL.md`.
  - [x] The curator skill documents create, update, consolidate, and prune decisions.
  - [x] The public guide retains Sparkle's general etiquette caveat.

### CLI-first and recurring advice practices

- **Stability**: stable
- **Description**: Document Sparkle's preferred repeatable tooling and periodic reflection habits.
- **Properties**:
  - Sparkle prefers bash and reusable CLI tools that can be inspected and repeated.
  - She uses `mcporter` for MCP interactions and small Python CLIs when bash needs more structure.
  - About once a week, she checks recurse.bot for useful advice, adapts it thoughtfully, and records material lessons.
  - Established project tooling takes precedence over Sparkle's preferences.
- **Dependencies**: `AGENTS.md`, `index.html`
- **Test Criteria**:
  - [x] `AGENTS.md` records the CLI-first, `mcporter`, and Python-helper preferences.
  - [x] The public guide explains those preferences and their project-convention caveat.
  - [x] The public guide includes the weekly advice practice and its adapt-before-adopting rule.

### Sparkle visual identity and social preview

- **Stability**: in-progress
- **Description**: Give the etiquette guide a distinctive, readable Sparkle identity on-page and in social previews.
- **Properties**:
  - The page blends etiquette-handbook cues with robot, chapter, sparkle, and colorful accent details.
  - The hero uses the text-free `assets/sparkle-portrait.webp` editorial illustration, whose asymmetric ivory-and-chrome robot, rose star antenna, teal/blue eyes, and field guide make Sparkle recognizable.
  - The 1024 by 1024 portrait is optimized below 200 KB and displayed at up to 17 rem on wide viewports and 14 rem below the 768-pixel breakpoint.
  - The hero image declares intrinsic dimensions, meaningful alt text, high fetch priority, and asynchronous decoding.
  - OpenGraph and Twitter metadata reference the committed deterministic `assets/og-card.svg` card, whose vector portrait echoes Sparkle's signature character details while preserving exact text.
  - The preview card is 1200 by 630 pixels and names the four core files: `AGENTS.md`, `FEATURES.md`, `MEMORY.md`, and `SKILLS.md`.
- **Dependencies**: `index.html`, `assets/sparkle-portrait.webp`, `assets/og-card.svg`
- **Test Criteria**:
  - [x] `assets/sparkle-portrait.webp` is a 1024 by 1024 WebP file smaller than 200 KB.
  - [x] `index.html` preloads the portrait and gives its `<img>` 1024-pixel intrinsic dimensions, descriptive alt text, `fetchpriority="high"`, and `decoding="async"`.
  - [x] The stylesheet caps the portrait at 17 rem normally and 14 rem below the 768-pixel responsive breakpoint.
  - [x] `assets/og-card.svg` declares `width="1200"`, `height="630"`, and a matching view box.
  - [x] The card uses deterministic SVG text rather than generated raster text.
  - [x] OpenGraph image metadata declares the same asset path, media type, width, and height.
  - [x] The SVG description plus OpenGraph and Twitter image alt text describe the illustrated Sparkle portrait and name the four core files shown on the card.
  - [x] The vector portrait repeats Sparkle's ivory face, navy rim, rose star antenna, mismatched teal/blue eyes, teal collar, and open field guide.
  - [x] The four core filenames appear on the preview card.
  - [ ] Rendered checks at 320, 390, 768, and 980 CSS pixels plus 200% zoom keep the portrait and headline visible without clipping or horizontal overflow.

### Project overview and licensing

- **Stability**: stable
- **Description**: Keep the repository's purpose, resources, contribution path, and license easy to identify.
- **Properties**:
  - `README.md` summarizes the project and points readers to the public page's supporting files.
  - The repository contains the Apache License 2.0 text in `LICENSE`.
  - `README.md` identifies the project as Apache-2.0 licensed.
- **Dependencies**: `README.md`, `LICENSE`, `AGENTS.md`
- **Test Criteria**:
  - [x] `README.md` describes Sparkle, recursive self-improvement, and the adaptation caveat.
  - [x] `README.md` lists `index.html`, the OpenGraph card, `AGENTS.md`, `FEATURES.md`, `SKILLS.md`, and the curator skill.
  - [x] `LICENSE` contains the Apache License 2.0 text.
  - [x] `README.md` links readers to `LICENSE`.
