# After Effects Expression Skill

مهارة Codex لتحويل أفكار الحركة المكتوبة باللغة الطبيعية إلى Expressions عملية في Adobe After Effects.

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## ما الذي تفعله

`$after-effects-expression` تجعل Codex يعمل كمصمم Expressions في After Effects. لا تعطي الكود فقط، بل توضح بنية الطبقات، عناصر التحكم المطلوبة، مكان لصق expression، الكود مع التعليقات، طريقة العمل، نقاط التعديل، والأخطاء المتوقعة.

## التثبيت

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## مثال

```text
$after-effects-expression
Create an expression that makes text scale up when a Null gets close, then return to normal.
```

يمكنك السؤال بلغتك، وسيحاول skill الرد بنفس اللغة.

## مناسب لـ

- proximity و effector rigs
- Position, Scale, Rotation, Opacity, Color, Source Text
- الحفاظ على keyframes الحالية باستخدام `value`
- `wiggle()`, `loopOut()`, `valueAtTime()`
- تفاعلات الصوت و markers
- عدادات النصوص
- تحويلات `toWorld()` و `toComp()`
- تصميم عناصر تحكم مناسبة لـ MOGRT
- إصلاح Expressions لا تعمل

## الحدود

Expressions تحسب قيم الخصائص فقط. لا تنشئ layers أو effects أو keyframes أو render jobs مباشرة. إذا احتاج الطلب إلى ذلك، تفصل المهارة بين الإعداد اليدوي، كود Expression، واحتمال استخدام JSX.

## الترخيص

MIT. راجع [LICENSE](../LICENSE).
