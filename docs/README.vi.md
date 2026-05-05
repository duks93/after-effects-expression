# After Effects Expression Skill

Một Codex skill giúp biến ý tưởng chuyển động bằng ngôn ngữ tự nhiên thành Adobe After Effects Expressions có thể dùng ngay.

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## Công dụng

`$after-effects-expression` giúp Codex trả lời như một người thiết kế Expression cho After Effects. Skill không chỉ đưa code, mà còn đưa cấu trúc layer, control cần thiết, nơi dán expression, code có chú thích, cách hoạt động, điểm tinh chỉnh và lỗi thường gặp.

## Cài đặt

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## Ví dụ

```text
$after-effects-expression
Tạo expression để text phóng to khi một Null tiến lại gần, rồi trở về kích thước ban đầu khi đi xa.
```

## Phù hợp cho

- proximity và effector rigs
- Position, Scale, Rotation, Opacity, Color, Source Text
- giữ keyframe hiện có bằng `value`
- `wiggle()`, `loopOut()`, `valueAtTime()`
- phản ứng theo audio và marker
- bộ đếm text
- label 2D bám theo layer 3D
- controller thân thiện với MOGRT
- sửa expression bị lỗi

## Giới hạn

Expression chỉ tính giá trị property. Nó không trực tiếp tạo layer, effect, keyframe, file hoặc render. Khi cần, skill sẽ tách phần setup thủ công, Expression code và hướng JSX tùy chọn.

## License

MIT. See [LICENSE](../LICENSE).
