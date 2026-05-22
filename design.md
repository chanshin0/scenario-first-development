<!--
design.md — 프로젝트 외관 자산 (네 서비스 소속, SFD 하네스 아님).

  정체성:
  - behavior 와 직교하는 외관 축. SoT(=scenarios/ Job Story) 는 그대로 — 이건 SoT 아님.
  - 게이트 아님 (soft guide). 누적 게이트 풀에 안 들어감.
  - goal(구현 시점)이 UI 코드를 쓸 때 이 토큰을 따르고, tweak(게이트2 시각 승인)이
    이 토큰을 판정 기준으로 인용한다.

  변경 규칙:
  - 아래 토큰 값 편집 = 프로젝트 작업 (자유 — scenarios 편집과 동급, sfd-architect 통로 밖).
  - goal/tweak 이 design.md 를 "어떻게 참조하는지"(메커니즘) 변경 = 하네스 → sfd-architect 통로.
-->

# Design Language (v0)

처음엔 최소로. 실제 구현에서 같은 결정이 반복될 때 한 줄씩 키운다 (과설계 금지 — 뭐가
필요한지 모르는 상태에서 토큰을 미리 채우지 않는다). 아래 값은 예시 — 네 서비스에 맞게 교체.

- **accent**: `#2563eb`
- **spacing**: `4px` 배수 (4 / 8 / 12 / 16 / 24)
- **font**: `system-ui`, `16px` base
- **radius**: `8px`
- **tone**: 담백하게, 느낌표 자제
