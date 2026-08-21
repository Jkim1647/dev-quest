# Release notes

## v0.2.0 — Award-quality polish candidate

발행일: 2026-08-21

공개 URL: https://wv1787202495138203.zaemit.ai/

### Changed

- 메인 페이지를 revision 34로 고도화
- Algorithm Dungeon 32, AI Laboratory 31, Project City 33 발행
- Hero 성장 루프와 Quest Console 고유 모티프 추가
- TODO를 의도적인 대기·잠금 상태로 교체
- World Map 연결 경로와 World별 색상 체계 적용
- 세 World의 4단계 운영 흐름 강화
- Journey, Achievements, Guestbook empty state 개선
- Footer 미등록 채널을 비활성 `Coming soon`으로 정리

### Preserved

- Guestbook 원본 데이터 시트
- 공개 승인 메시지용 공개 시트
- 읽기 전용 목록 API
- 공개 API 필드 `nickname`, `message`, `published_at`
- 실제 데이터가 없을 때 가짜 테스트 메시지를 넣지 않는 정책

### QA

- 공개 URL과 4개 주요 페이지 비로그인 조회
- DOM 가로 넘침 0px
- 1024px / 768px / 390px 규칙과 360px 상속
- 키보드 포커스, heading 구조, reduced motion
- 주요 상호작용 영역 44px 이상
- CTA, 앵커, World Map 링크
- Guestbook 필수·선택 동의와 공개 목록 빈 상태

### Remaining before submission

- 실제 모바일 기기 스크롤 감각 확인
- 제출용 화면 캡처 보관
- 임시 도메인의 SEO 렌더링 문제 재확인
- 공모전 Google Forms 최종 제출

## v0.1.0 — Contest submission candidate

발행일: 2026-08-20

- DEV QUEST 기본 정보 구조와 World Map 구축
- 세 개의 World 페이지와 Guestbook 데이터 구조 구현
- SEO, AEO, AI crawler, `llms.txt` 설정
- 첫 공개 QA 및 프로젝트 기록 저장소 생성
