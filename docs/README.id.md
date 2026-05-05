# After Effects Expression Skill

Skill Codex untuk mengubah ide motion dalam bahasa natural menjadi Adobe After Effects Expressions yang siap dipakai.

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## Fungsi

`$after-effects-expression` membuat Codex menjawab seperti desainer Expression After Effects. Outputnya mencakup struktur layer, kontrol yang dibutuhkan, lokasi paste expression, kode dengan komentar, cara kerja, nilai yang bisa diatur, dan pencegahan error.

## Instalasi

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## Contoh

```text
$after-effects-expression
Buat expression agar teks membesar saat Null mendekat, lalu kembali normal saat menjauh.
```

## Cocok Untuk

- proximity dan effector rigs
- Position, Scale, Rotation, Opacity, Color, Source Text
- mempertahankan keyframe dengan `value`
- `wiggle()`, `loopOut()`, `valueAtTime()`
- reaksi audio dan marker
- text counter
- label 2D yang mengikuti layer 3D
- controller untuk MOGRT
- debugging expression yang error

## Batasan

Expression menghitung nilai property. Expression tidak membuat layer, effect, keyframe, file, atau render secara langsung. Jika diperlukan, skill akan memisahkan setup manual, kode Expression, dan opsi JSX.

## Lisensi

MIT. Lihat [LICENSE](../LICENSE).
