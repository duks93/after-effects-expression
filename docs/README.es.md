# After Effects Expression Skill

Convierte ideas de movimiento escritas en lenguaje natural en expresiones prácticas para Adobe After Effects.

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## Qué hace

`$after-effects-expression` convierte Codex en un asistente especializado en expresiones de After Effects. Entrega la estructura de capas, controles necesarios, propiedad exacta donde pegar la expresión, código comentado, explicación, puntos de ajuste y prevención de errores.

## Instalación

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## Ejemplo

```text
$after-effects-expression
Crea una expresión para que un texto crezca cuando un Null se acerque y vuelva a su tamaño original al alejarse.
```

## Casos ideales

- rigs de proximidad y effector
- Position, Scale, Rotation, Opacity, Color, Source Text
- expresiones que conservan keyframes existentes
- `wiggle()`, `loopOut()`, `valueAtTime()`
- audio, markers, contadores de texto
- etiquetas 2D que siguen capas 3D
- diseño de controles para MOGRT
- depuración de expresiones rotas

## Límite importante

Las expresiones calculan valores de propiedades. No crean capas, efectos, keyframes, archivos ni renders por sí solas. Cuando sea necesario, el skill separa la configuración manual, la expresión y una posible solución con JSX.

## Licencia

MIT. Consulta [LICENSE](../LICENSE).
