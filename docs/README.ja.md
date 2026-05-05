# After Effects Expression Skill

Natural-language motion ideas can become practical Adobe After Effects expressions with this Codex skill.

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## これは何ですか

`$after-effects-expression` は、Codex を After Effects Expression の設計者、モーショングラフィックスのリギング支援者として使うためのスキルです。

コードだけではなく、レイヤー構成、Expression Controls、貼り付けるプロパティ、コメント付きコード、調整ポイント、エラー対策まで提示します。

## インストール

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## 使い方

```text
$after-effects-expression
Create an expression that makes text scale up when a Null gets close.
```

日本語で依頼しても構いません。

```text
$after-effects-expression
Null が近づくとテキストが大きくなり、離れると元に戻る Expression を作って。
```

## 得意な用途

- proximity / effector rigs
- Position, Scale, Rotation, Opacity, Color, Source Text
- `wiggle()`, `loopOut()`, `valueAtTime()`
- audio and marker reactions
- text counters and text-box rigs
- `toWorld()` distance calculation
- `toComp()` 3D-to-2D labels
- MOGRT-friendly controllers
- debugging broken expressions

## 基本方針

情報が足りない場合でも、質問だけで終わりません。一般的な AE 構成を仮定し、まず動く Expression を提示してから、より精密にするための質問をします。

## ライセンス

MIT. See [LICENSE](../LICENSE).
