# After Effects Expression Skill

Transformez une idée de mouvement en langage naturel en expression Adobe After Effects prête à coller.

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## Objectif

`$after-effects-expression` aide Codex à répondre comme un concepteur d'expressions After Effects. Il fournit le plan de calques, les Expression Controls, l'endroit exact où coller le code, le code commenté, l'explication, les réglages et les erreurs fréquentes.

## Installation

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## Exemple

```text
$after-effects-expression
Crée une expression pour qu'un texte grossisse quand un Null s'approche, puis revienne à sa taille normale.
```

## Utilisations recommandées

- proximité et effector rigs
- Position, Scale, Rotation, Opacity, Color, Source Text
- conservation des keyframes avec `value`
- `wiggle()`, `loopOut()`, `valueAtTime()`
- réactions audio et markers
- compteurs de texte
- conversions `toWorld()` et `toComp()`
- contrôleurs MOGRT
- correction d'expressions existantes

## Principe

Quand des informations manquent, le skill formule des hypothèses raisonnables et donne une première version fonctionnelle avant de poser des questions.

## Licence

MIT. Voir [LICENSE](../LICENSE).
