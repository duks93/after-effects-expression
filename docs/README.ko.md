# After Effects Expression Skill

자연어로 말한 모션 아이디어를 실제 After Effects에 붙여 넣을 수 있는 Expression으로 바꿔 주는 Codex 스킬입니다.

[English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português BR](README.pt-BR.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md)

## 무엇을 해주나

`$after-effects-expression`은 Codex를 After Effects Expression 설계자처럼 동작하게 만듭니다. 단순 코드 조각만 주는 것이 아니라 레이어 구조, 컨트롤, 적용 속성, 주석 포함 코드, 작동 원리, 조정 포인트, 오류 예방까지 함께 제공합니다.

## 설치

```bash
git clone https://github.com/duks93/after-effects-expression.git ~/.codex/skills/after-effects-expression
```

## 사용 예시

```text
$after-effects-expression
Null이 가까이 오면 텍스트가 커지고 멀어지면 원래 크기로 돌아오는 expression 만들어줘.
```

## 잘 맞는 작업

- 거리 기반 Proximity / Effector 반응
- Position, Scale, Rotation, Opacity, Color, Source Text 제어
- 키프레임 유지와 `value` 기반 보정
- `wiggle()`, `loopOut()`, `valueAtTime()` 패턴
- 오디오 반응, 마커 반응, 텍스트 카운터
- 3D 레이어를 2D 라벨이 따라가는 `toComp()` 구조
- 부모/프리컴프/3D가 섞인 `toWorld()` 거리 계산
- MOGRT용 컨트롤러 설계
- 기존 Expression 오류 수정

## 답변 방식

스킬은 보통 다음 순서로 답합니다.

1. 요청 해석
2. 기본 가정
3. AE 세팅 순서
4. 필요한 컨트롤
5. Expression 코드
6. 작동 원리
7. 조정 포인트
8. 오류 예방
9. 추가 질문

정보가 부족해도 질문만 하지 않고, 가장 일반적인 AE 환경을 가정해 먼저 작동 가능한 1차 버전을 제공합니다.

## 한계

Expression은 속성 값을 계산합니다. 레이어 생성, 효과 추가, 키프레임 생성, 저장, 렌더, 일괄 적용은 Expression만으로 직접 수행하지 않습니다. 그런 요청은 수동 AE 세팅, Expression, 필요 시 JSX 스크립트로 나누어 안내합니다.

## 업데이트

```bash
cd ~/.codex/skills/after-effects-expression
git pull
```

## 라이선스

MIT. 자세한 내용은 [LICENSE](../LICENSE)를 확인하세요.
