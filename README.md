# DEV QUEST

> Build. Solve. Learn. Repeat.

알고리즘, AI, 프로젝트를 공부하며 성장하는 과정을 RPG의 Quest와 World Map처럼 기록하는 장기 운영형 **Developer Growth Archive**입니다.

## Live site

- Production: https://wv1787202495138203.zaemit.ai/
- Platform: [Zaemit](https://zaemit.ai/)
- Current milestone: `v0.2.0 — Award-quality polish candidate`

## Contest

- **공모전명:** 내 AI와 만드는 디자인 웹사이트 공모전
- **주최:** 위븐
- **접수 기간:** 2026-08-19 ~ 2026-09-18
- **참여 대상:** 제한 없음
- **분야:** 디자인 / 순수미술 / 공예
- **추가 혜택:** iPad Air
- **공고:** [링커리어 공고 보기](https://linkareer.com/activity/344044)

세부 공고 정보와 제출 체크리스트는 [`docs/CONTEST.md`](docs/CONTEST.md)를 참고하세요.

## Why DEV QUEST?

일반적인 이력서형 포트폴리오보다 개발자가 되어가는 과정 자체에 집중합니다. 문제 해결, 개념 학습, 프로젝트 구현, 회고와 성취가 하나의 성장 세계로 연결되며 실제 기록이 쌓일수록 사이트도 함께 확장됩니다.

## Information architecture

- **Hero / Current Status** — 사이트 목적과 현재 성장 상태
- **Current Quest** — 가장 중요한 학습 또는 개발 목표
- **World Map** — 세 가지 핵심 성장 영역
  - Algorithm Dungeon
  - AI Laboratory
  - Project City
- **Journey** — 시간에 따른 성장 체크포인트
- **Achievements** — 근거가 있는 성취만 해금되는 기록
- **Guestbook** — 방문자 메시지와 공개 동의 기반 Recent Traces

## Key principles

- 존재하지 않는 경력, 성과, 프로젝트, 학습 수치를 만들지 않습니다.
- 실제 데이터가 없을 때는 의도적인 empty/locked state를 사용합니다.
- 게임 UI는 세계관을 전달하는 수준으로 절제하고 포트폴리오 가독성을 우선합니다.
- Desktop, Tablet, Mobile과 키보드 탐색, reduced motion을 지원합니다.
- Zaemit 데이터 시트와 API를 이용해 공모전 이후에도 운영 가능한 구조를 유지합니다.

## Zaemit features used

- Zaemit MCP를 통한 사이트·페이지·컴포넌트 생성 및 수정
- Header / Footer와 반응형 내비게이션
- Algorithm, AI, Project 하위 페이지
- Guestbook 원본 데이터 시트
- 공개 동의 메시지용 별도 공개 시트와 읽기 전용 API
- SEO, canonical, AEO, AI crawler, `llms.txt` 설정
- 공개 페이지 재발행 및 비로그인 검증

### v0.2.0 polish

- Hero에 성장 루프와 Quest Console 모티프 적용
- World Map 연결 경로와 World별 색상 체계 강화
- Algorithm / AI / Project의 4단계 운영 흐름 정교화
- TODO 문구를 의도적인 대기·잠금 상태로 교체
- Journey, Achievements, Guestbook empty state 개선
- 미등록 Footer 채널을 비활성 `Coming soon` 상태로 정리
- 1024px / 768px / 390px 반응형 규칙과 360px 상속 검증

자세한 내역은 [`docs/MCP_WORKLOG.md`](docs/MCP_WORKLOG.md)를 참고하세요.

## Repository scope

이 저장소는 Zaemit에서 관리되는 사이트의 **프로젝트 기록 및 버전 체크포인트**입니다. 현재 Zaemit은 편집 가능한 전체 프로젝트 소스의 Git 내보내기를 제공하지 않아, 실제 배포 소스 대신 구조·결정·QA·운영 계획을 버전 관리합니다.

## Documentation

- [`docs/PROJECT_STATUS.md`](docs/PROJECT_STATUS.md) — 1차 제작 현황
- [`docs/MCP_WORKLOG.md`](docs/MCP_WORKLOG.md) — Zaemit MCP 수행 기록
- [`docs/QA_REPORT.md`](docs/QA_REPORT.md) — 공개 사이트 QA
- [`docs/ROADMAP.md`](docs/ROADMAP.md) — 2차 개선 계획
- [`docs/SUBMISSION.md`](docs/SUBMISSION.md) — 공모전 제출용 설명
- [`docs/CONTEST.md`](docs/CONTEST.md) — 공모전 개요와 제출 체크리스트
- [`docs/RELEASE_NOTES.md`](docs/RELEASE_NOTES.md) — 버전별 변경 기록

## License

Copyright © 2026. All rights reserved. 콘텐츠와 디자인의 재사용 허가는 별도로 문의해 주세요.
