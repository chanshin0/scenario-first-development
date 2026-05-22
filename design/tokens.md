<!--
design/tokens.md — 외관 '값'의 단일 SoT (네가 편집하는 원본).

  - 값은 여기에만. design.md(말)·생성물(tokens.css/theme.css)에 값을 중복하지 않는다.
  - goal 이 이 파일을 읽어 스택 맞는 코드를 생성한다 (순수 CSS → :root / Tailwind → @theme).
  - 값 편집 = 프로젝트 작업 (자유, sfd-architect 통로 밖). 고치면 goal/tweak 이 생성물 재생성.
  - 아래는 v0 예시 — 네 서비스 값으로 교체.
-->

# Design Tokens (v0)

## Color
- accent: `#2563eb`
- danger: `#dc3545`
- success: `#198754`
- text: `#212529`
- muted: `#6c757d`
- border: `#ced4da`
- bg: `#f8f9fa`

## Spacing
- base: `4px` (배수: 4 / 8 / 12 / 16 / 24)

## Typography
- font: `system-ui`
- size-base: `16px`

## Radius
- radius: `8px`

---

> 토큰 **값** 변경(색·간격…)은 외관만 바뀌므로 누적 게이트 풀(행동) green 을 유지한다 → tweak 영역.
> 단 **색 자체가 유일한 의미 전달**이면(예: 빨강=실패, 초록=성공을 색으로만 구분) 그건 행동이라 tweak 아님 → `deepen` (그리고 GWT 는 색이 아닌 text/role/aria 로 단언).
