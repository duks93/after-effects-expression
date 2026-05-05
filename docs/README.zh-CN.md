# After Effects Expression Skill

这个 Codex 技能可以把自然语言描述的动效需求转换成可直接粘贴到 Adobe After Effects 的 Expression。

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## 功能

`$after-effects-expression` 让 Codex 像 After Effects Expression 设计师一样回答。它不仅给代码，还会说明图层结构、控制器、粘贴位置、注释代码、工作原理、可调参数和常见错误。

## 安装

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## 示例

```text
$after-effects-expression
Create an expression that makes a 2D label follow a 3D layer on screen.
```

也可以用中文提问：

```text
$after-effects-expression
Null 靠近文字时让文字变大，远离时恢复原始大小。
```

## 适合的任务

- 距离感应和 Effector 动效
- Position, Scale, Rotation, Opacity, Color, Source Text
- 保留已有关键帧的表达式
- `wiggle()`, `loopOut()`, `valueAtTime()`
- 音频、Marker、文本计数器
- `toWorld()` 和 `toComp()` 坐标转换
- MOGRT 控制器设计
- 修复错误 Expression

## 边界

Expression 负责计算属性值。它不能直接创建图层、添加效果、生成关键帧、保存文件或执行渲染。如果任务需要这些操作，技能会把手动设置、Expression 和可选 JSX 脚本分开说明。

## License

MIT. See [LICENSE](../LICENSE).
