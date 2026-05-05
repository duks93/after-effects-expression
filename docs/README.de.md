# After Effects Expression Skill

Dieses Codex-Skill verwandelt natürlich formulierte Motion-Ideen in praxistaugliche Adobe After Effects Expressions.

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## Zweck

`$after-effects-expression` lässt Codex wie einen After-Effects-Expression-Designer antworten. Es liefert nicht nur Code, sondern auch Layer-Struktur, benötigte Controls, Einfügeposition, kommentierten Code, Erklärung, Einstellpunkte und typische Fehlerquellen.

## Installation

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## Beispiel

```text
$after-effects-expression
Erstelle eine Expression, bei der ein Text größer wird, wenn ein Null näherkommt, und wieder normal wird, wenn es weggeht.
```

## Geeignet für

- Proximity- und Effector-Rigs
- Position, Scale, Rotation, Opacity, Color, Source Text
- bestehende Keyframes mit `value` erhalten
- `wiggle()`, `loopOut()`, `valueAtTime()`
- Audio- und Marker-Reaktionen
- Textzähler und Textbox-Rigs
- `toWorld()` und `toComp()` Koordinatenumrechnung
- MOGRT-freundliche Controller
- Debugging fehlerhafter Expressions

## Grenze

Expressions berechnen Property-Werte. Sie erstellen keine Layer, Effekte, Keyframes, Dateien oder Render-Jobs. Wenn nötig, trennt das Skill manuelle AE-Schritte, Expression-Code und optionale JSX-Hinweise.

## Lizenz

MIT. Siehe [LICENSE](../LICENSE).
