# After Effects Expression Skill

यह Codex skill प्राकृतिक भाषा में लिखे motion ideas को Adobe After Effects में इस्तेमाल होने वाले practical Expressions में बदलने के लिए है।

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## यह क्या करता है

`$after-effects-expression` Codex को After Effects Expression designer की तरह जवाब देने में मदद करता है। यह केवल code नहीं देता, बल्कि layer setup, required controls, paste location, commented expression, explanation, adjustment points और troubleshooting भी देता है।

## Install

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## Example

```text
$after-effects-expression
Null पास आने पर text बड़ा हो और दूर जाने पर normal size में लौट आए, ऐसी expression बनाओ.
```

## Useful For

- proximity और effector rigs
- Position, Scale, Rotation, Opacity, Color, Source Text
- existing keyframes को `value` से preserve करना
- `wiggle()`, `loopOut()`, `valueAtTime()`
- audio और marker reactions
- text counters
- 3D layer को follow करने वाले 2D labels
- MOGRT-friendly controller design
- broken expressions debug करना

## Limit

Expressions property values calculate करती हैं। वे layers, effects, keyframes, files या renders खुद create नहीं करतीं। जरूरत होने पर skill manual setup, Expression code और optional JSX direction को अलग-अलग बताती है।

## License

MIT. See [LICENSE](../LICENSE).
