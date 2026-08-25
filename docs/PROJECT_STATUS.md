# Project status — v0.2.0

기준일: 2026-08-21

공개 URL: https://wv1787202495138203.zaemit.ai/

## 완료된 범위

- DEV QUEST 브랜드와 Hero
- `Build. Solve. Learn. Repeat.` 슬로건
- Current Status / Current Quest
- World Map과 세 개의 하위 페이지
- Algorithm Dungeon
- AI Laboratory
- Project City
- Journey Timeline
- Achievement locked states
- Guestbook 저장 폼
- 메시지 공개 동의 필드
- 공개 승인 메시지만 읽는 Recent Traces API/UI
- Header, Footer, 모바일 내비게이션
- 반응형 CSS, 키보드 포커스, reduced motion
- canonical, AEO, AI crawler, `llms.txt` 설정
- Hero 성장 루프와 Quest Console 모티프
- World Map 연결 경로와 World별 색상 체계
- Algorithm, AI, Project의 4단계 운영 흐름
- TODO를 대기·잠금 상태로 교체
- Journey, Achievements, Guestbook empty state 개선
- Footer 미등록 채널의 비활성 `Coming soon` 처리

## 현재 활성 page sequence

| 대상 | Page sequence |
| --- | ---: |
| Main | 68 |
| Algorithm Dungeon | 35 |
| AI Laboratory | 36 |
| Project City | 37 |
| MY QUEST | 65 |

공통 Header와 Footer는 수정 후 복구 이력을 생성했으며, Guestbook 원본·공개 시트와 API 구조는 변경하지 않았습니다.

## 데이터 정책

- 경력·프로젝트·학습 수치·수상 기록을 임의 생성하지 않았습니다.
- 현재 실제 방명록 데이터는 0건입니다.
- Algorithm, AI, Project 시트에는 사용법 안내용 DEMO 기록이 각각 1건 있습니다.
- DEMO 기록은 제목과 작성자에 명시적으로 표시하며 실제 성과로 계산하지 않습니다.
- 개인정보 동의는 필수이며 메시지 공개 동의는 선택입니다.
- 공개 API에는 `nickname`, `message`, `published_at`만 노출합니다.
- MY QUEST 데이터는 별도 `sd_my_quest_records` 시트에 저장합니다.
- MY QUEST API 5종은 모두 `member_scope: 1`이며 현재 개인 데이터는 0건입니다.
- 개인 Quest는 생성 요청에서 `is_public=false`를 명시합니다.

## 회원 기능

- 비로그인: DEMO QUEST, World Map, Guestbook 이용
- 로그인: 개인 Quest 생성, 목록 조회, 수정, 완료, 삭제
- 공식 로그인·회원가입·마이페이지 경로 연결
- same-origin 회원 세션 사용
- 프런트엔드 API 키와 `localStorage` 미사용
- 운영자 공개 기록과 회원 개인 기록의 시트 분리

## 알려진 플랫폼 제약

- Zaemit 임시 도메인은 공개 HTML에 `noindex,nofollow`를 강제합니다.
- 공식 SEO 설정에 저장된 Description이 임시 도메인 HTML에는 반영되지 않고 본문이 자동 추출됩니다.
- 현재 MCP의 공식 SEO 도구에는 OG image와 페이지별 Description 지정 필드가 없습니다.
- 공식 파비콘 연결은 Zaemit 관리 UI에서 직접 선택해야 합니다.
- 커스텀 도메인, 검색엔진 소유 확인, 외부 분석 도구 연결은 아직 진행하지 않았습니다.

## 공모전 필수 조건

- 공모전: 내 AI와 만드는 디자인 웹사이트 공모전
- 주최: 위븐
- 접수 기간: 2026-08-19 ~ 2026-09-18
- 공고: https://linkareer.com/activity/344044

- [x] 접수 기간 내 Zaemit으로 제작
- [x] Zaemit MCP 실제 사용
- [x] 공개 URL 발행
- [x] 비로그인 접속 가능
- [x] 공모전 이후 운영 가능한 구조
- [ ] 최종 Google Forms 제출 — 사용자가 직접 수행
