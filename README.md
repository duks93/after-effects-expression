# After Effects Expression Skill

Turn natural-language motion ideas into production-ready Adobe After Effects expressions.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Codex Skill](https://img.shields.io/badge/Codex-Skill-111827.svg)](SKILL.md)
[![After Effects](https://img.shields.io/badge/Adobe-After%20Effects-9999FF.svg)](https://www.adobe.com/products/aftereffects.html)

Repository: [duks93/after-effects-expression](https://github.com/duks93/after-effects-expression)

Languages:
[English](README.md) ·
[한국어](docs/README.ko.md) ·
[日本語](docs/README.ja.md) ·
[简体中文](docs/README.zh-CN.md) ·
[Español](docs/README.es.md) ·
[Français](docs/README.fr.md) ·
[Deutsch](docs/README.de.md) ·
[Português BR](docs/README.pt-BR.md) ·
[العربية](docs/README.ar.md) ·
[हिन्दी](docs/README.hi.md) ·
[Bahasa Indonesia](docs/README.id.md) ·
[Tiếng Việt](docs/README.vi.md)

This skill makes Codex behave like an After Effects expression designer, motion-graphics rigging engineer, and template assistant. It does not only produce code. It gives the layer structure, Expression Controls, paste location, annotated expression, return type, adjustment points, and troubleshooting guidance a real AE user needs.

## What It Is For

Use `$after-effects-expression` when you want to:

- convert plain-language motion requests into copy-pasteable expressions
- debug an existing expression that fails in After Effects
- design controller layers and Expression Controls
- build proximity, effector, audio, marker, text, 2D/3D, MOGRT, or keyframe-based rigs
- explain exactly where to paste an expression and what AE setup is required

The skill is optimized for practical work: it assumes missing details, gives a working first version, and then asks useful follow-up questions.

## Quick Start

Install into your Codex skills directory:

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

Then ask Codex:

```text
$after-effects-expression
After Effects에서 Null이 가까이 오면 텍스트가 커지고 멀어지면 원래 크기로 돌아오는 expression 만들어줘.
```

Or in English:

```text
$after-effects-expression
Create an After Effects expression that makes a 2D label follow a 3D layer on screen.
```

## Recommended First Test

Ask for a simple proximity expression:

```text
$after-effects-expression
Make a layer scale up when it gets close to a Null called "Effector".
```

A good answer should include:

- the exact property, usually `Transform > Scale`
- a clear AE setup sequence
- any required controls and default values
- real After Effects expression syntax
- comments inside the code
- return-type and dimension warnings
- troubleshooting for layer/control names

## How The Skill Thinks

The skill follows a stable hierarchy:

1. Interpret the motion request as After Effects layers, properties, time, distance, controls, keyframes, audio, markers, text, or coordinate systems.
2. Decide the target layer, reference layer, property, 2D/3D dimension, existing keyframe behavior, and return type.
3. Specify the AE setup before the code.
4. Write copy-pasteable Expression code.
5. Explain how it works and what values to adjust.
6. Add likely error fixes.
7. Ask follow-up questions only after giving a useful first version.

## Supported Expression Patterns

The bundled references cover:

- time-based animation
- `wiggle()` and stable randomization
- `loopIn()` / `loopOut()` keyframe loops
- staggered delay with `index`
- proximity and effector rigs
- repel / attract / scale / opacity / color reactions
- `Audio Amplitude` driven motion
- marker-triggered animation
- text counters and `Source Text`
- `sourceRectAtTime()` text-box rigs
- `toWorld()` parent-safe distance calculations
- `toComp()` 3D-to-2D screen labels
- Checkbox and Dropdown Control mode switching
- MOGRT-friendly controller design

## Repository Structure

```text
after-effects-expression/
├── SKILL.md
├── LICENSE
├── README.md
├── agents/
│   └── openai.yaml
├── docs/
│   └── README.*.md
└── references/
    ├── pattern-index.md
    ├── response-hierarchy.md
    └── full-project-prompt.md
```

`SKILL.md` stays concise so Codex can load the workflow quickly. Detailed expression patterns live under `references/` and are loaded only when needed.

## Boundaries

After Effects Expressions calculate property values. They can control Position, Scale, Rotation, Opacity, Color, Source Text, timing, distance, audio, markers, and coordinate conversions.

Expressions do not directly create layers, add effects, generate keyframes, save project files, run renders, or batch-apply themselves. If a request needs those actions, the skill separates:

- manual AE setup
- Expression code
- optional JSX scripting direction

## Example Request

```text
$after-effects-expression
I have many text layers. When a Null passes near each text layer, the text should move upward, scale up, and fade in smoothly. Keep existing keyframes.
```

The skill should return a practical rig plan using a controller or Effector layer, `toWorld()` distance checks, `linear()` / `ease()` / `clamp()`, and `value` preservation.

## Updating

```bash
cd ~/.codex/skills/after-effects-expression
git pull
```

## Contributing

Issues and pull requests are welcome. The best contributions are:

- tested expression patterns
- clearer troubleshooting notes
- language improvements
- examples from real AE workflows

Keep the skill lightweight. Put reusable details in `references/` instead of expanding `SKILL.md` unnecessarily.

## License

MIT. See [LICENSE](LICENSE).
