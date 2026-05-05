# After Effects Expression Skill

Transforme ideias de movimento escritas em linguagem natural em expressões práticas para Adobe After Effects.

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## O que é

`$after-effects-expression` faz o Codex responder como um designer de Expressions do After Effects. Ele entrega estrutura de layers, controles, propriedade exata para colar o código, expressão comentada, explicação, ajustes e prevenção de erros.

## Instalação

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## Exemplo

```text
$after-effects-expression
Crie uma expression para o texto aumentar quando um Null se aproximar e voltar ao tamanho original quando se afastar.
```

## Bons usos

- proximity e effector rigs
- Position, Scale, Rotation, Opacity, Color, Source Text
- preservar keyframes existentes com `value`
- `wiggle()`, `loopOut()`, `valueAtTime()`
- reações a áudio e markers
- contadores de texto
- labels 2D seguindo layers 3D
- controles para MOGRT
- correção de expressions com erro

## Limite

Expressions calculam valores de propriedades. Elas não criam layers, efeitos, keyframes, arquivos ou renders. Quando necessário, o skill separa configuração manual, código Expression e possível caminho com JSX.

## Licença

MIT. Veja [LICENSE](../LICENSE).
