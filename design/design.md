<!--
design/design.md — 프로젝트 외관의 '말'(원칙·톤·이유). 네 서비스 소속, SFD 하네스 아님.

  이 폴더(design/)의 분업:
  - design.md  = 말   : 왜 이렇게, 어떤 톤, 언제 뭘 쓰나 (사람·Claude 가 읽고 판단)
  - tokens.md  = 값   : 색·간격·radius 등 숫자의 단일 SoT (네가 편집하는 원본)
  - tokens.css/theme.css = 생성물 : goal 이 tokens.md 에서 스택 맞춰 만든 코드 (직접 편집 금지)

  정체성:
  - behavior 와 직교하는 외관 축. SoT(=scenarios/ Job Story) 는 그대로 — 이건 SoT 아님.
    (tokens.md 는 외관 '값'의 SoT 일 뿐, behavior SoT 아님.)
  - 게이트 아님 (soft guide). 누적 게이트 풀에 안 들어감.
  - goal(구현 시점)이 tokens.md 를 코드로 생성·사용하고, tweak(게이트2 시각 승인)이
    design.md(톤)+tokens.md(값)를 판정 기준으로 인용한다.

  변경 규칙:
  - design.md 톤·원칙 / tokens.md 값 편집 = 프로젝트 작업 (자유 — scenarios 편집과 동급, 통로 밖).
  - goal/tweak 이 이 파일들을 "어떻게 참조·생성하는지"(메커니즘) 변경 = 하네스 → sfd-architect 통로.
-->

# Design Language (v0)

이 파일은 **말**이다 — 값(숫자)은 `tokens.md` 에 있다. 여긴 *왜 그렇게 정했나*, *어떤 톤인가*, *언제 뭘 쓰나* 만 적는다. 처음엔 최소로, 결정이 반복될 때 한 줄씩 키운다 (과설계 금지).

## 톤 (시드 — 네 서비스에 맞게 교체)

- 담백하게, 느낌표 자제.
- accent 색은 주요 액션(주 버튼·링크)에만. 남발 금지.
- 여백은 넉넉히 — 빽빽하게 채우지 않는다.

## 값은 어디에

색·간격·폰트·radius 같은 **값은 `design/tokens.md`** 에 있다 (단일 원본). goal 이 그걸 읽어 스택에 맞는 코드(`tokens.css` :root / `theme.css` @theme)로 **생성**하고, 코드는 그 변수(`var(--accent)` 등)를 쓴다. 값을 바꾸려면 `tokens.md` 만 고치고 재생성 — design.md 에 값을 다시 적지 않는다 (중복 = 표류).

> **생성물 위치**: (아직 없음 — goal 이 tokens.md 에서 생성)
