# Photo Collage World

**Photo Collage World** is an AI image-creation Skill for transforming real photographs into complete, theme-driven collage worlds.

It is not a filter and not a simple "photo + decorations" workflow.

The core method is to extract the source image's subject, relationships, colors, shapes, textures, atmosphere, and thematic cues, then rebuild the surrounding visual world around them.

## Core Philosophy

### Preserve the story, not the environment

The most important information in a photograph is its story, subject, and key relationships. The original environment does not need to remain unchanged.

### Preserve relationships, not every object

The Skill does not mechanically preserve every visible object.

For example:

> pavilion + tree + water

may become:

> geometric pavilion structure + botanical texture + large color field representing water

as long as the core relationship remains recognizable.

### Build a world, not a decoration layer

The goal is a complete visual system derived from the original photograph.

Reference images provide visual language such as:

- composition
- color relationships
- spatial hierarchy
- graphic language
- scale relationships
- collage rhythm

They do **not** provide a fixed template.

## Features

- Preserve the recognizable primary subject
- Reconstruct the surrounding environment
- Build a theme-driven visual world
- Use large / medium / small visual hierarchy
- Treat color as a compositional tool
- Use controlled secondary creativity
- Avoid fixed reference-image motifs
- Adapt subject protection to portraits, food, landscapes, night scenes, and other source types
- Balance creative transformation with source recognizability

## Repository Structure

```text
photo-collage-world/
├── SKILL.md
├── README.md
├── LICENSE
├── agents/
│   └── openai.yaml
├── references/
│   ├── visual-language.md
│   ├── composition.md
│   ├── subject-protection.md
│   └── examples.md
└── examples/
```

## Usage

Provide this Skill to a Skills-compatible AI agent and give it a real photograph.

The core instruction is:

> Transform this photograph into a complete, theme-driven collage world while preserving the source image's core story, recognizable primary subject, and key visual relationships.

The amount of transformation should depend on the source image.

The environment may change dramatically. The core subject and story should not disappear.

## Design Goal

Avoid both extremes.

**Under-reconstruction**

> Real photograph + a few decorative elements

**Over-reconstruction**

> The original story and subject can no longer be identified

**Target**

> The original story remains recognizable while the environment, spatial structure, color system, and visual language are substantially and intentionally redesigned.

## Multiple Generation Attempts

Different generations can produce meaningfully different compositions, color systems, and creative interpretations.

Whether to make additional attempts is **up to the user**.

If the first result is technically correct but visually weak, a second or third generation may produce a stronger interpretation.

The Skill does not require repeated generation automatically.

## License

MIT License
