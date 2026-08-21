# QA report — v0.2.0 polish

기준일: 2026-08-21

근거: Zaemit MCP 작업 결과 및 공개 비로그인 브라우저 QA 기록

## Public routes

| Route | Result |
|---|---|
| `/` | HTTP 200 |
| `/page/dev-quest/` | HTTP 200 |
| `/page/algorithm-dungeon` | HTTP 200 |
| `/page/ai-laboratory` | HTTP 200 |
| `/page/project-city` | HTTP 200 |

## Verified

- Home title: `DEV QUEST | Developer Journey`
- Home H1: `DEV QUEST`
- Header와 반응형 메뉴
- CTA와 내부 앵커
- World Map 하위 페이지 링크
- Guestbook 필수 입력과 개인정보 동의
- 선택형 메시지 공개 동의
- 공개 승인 메시지용 읽기 전용 API
- 실제 데이터가 없을 때의 empty state
- Footer의 브랜드와 `Made with AI & Zaemit`
- 키보드 포커스 2px cyan outline
- 데스크톱 가로 넘침 없음
- 주요 CTA와 내비게이션의 44px 이상 터치 영역
- 991px / 767px 반응형 규칙
- `prefers-reduced-motion` 지원
- 공개 DOM 가로 넘침 `0px`
- 1024px / 768px / 390px 미디어 규칙과 360px 상속
- 모바일 좌우 여백 `20px`
- 주요 탐색, 버튼, 동의 레이블의 44px 이상 터치 영역
- heading 구조와 `aria-live` 빈 상태
- Guestbook 필수 개인정보 동의와 선택 공개 동의
- 공개 API 노출 필드: `nickname`, `message`, `published_at`
- 테스트 메시지 미저장

## Known limitations

- 공개 HTML robots: `noindex,nofollow` — 임시 Zaemit 도메인 정책
- Description과 OG Description: 본문 자동 추출 — 임시 도메인 생성기 제약
- OG image 태그 없음 — 현재 공식 MCP 도구 필드 미제공
- `/favicon.ico` 사용 중이나 관리 UI의 공식 파비콘 체크 미완료
- 실제 모바일 기기의 최종 스크롤 감각은 제출 전에 직접 확인 필요

## Release decision

공개성, MCP 사용, 정보 구조, 반응형·접근성 규칙, 실제 운영 기능이 유지된 공모전 제출 후보 상태입니다. 플랫폼 SEO 제약은 관리자 지원 또는 커스텀 도메인 연결 환경에서 최종 확인해야 합니다. 공모전 접수는 아직 수행하지 않았습니다.
