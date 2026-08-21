# MY QUEST

공개 포트폴리오와 분리된 회원 전용 개발 성장 기록 공간입니다.

## User journeys

### Guest

- QUEST REPLAY DEMO 체험
- World Map과 공개 성장 기록 탐색
- Guestbook 작성
- MY QUEST 저장 시 공식 로그인 안내

### Member

- Algorithm, AI, Project 중 World 선택
- 4단계 Stepper로 사고 과정 작성
- 임시 저장, 목록 조회, 수정, 완료, 삭제
- 기본 비공개 상태로 개인 기록 관리

## Data model

- Sheet: `MY QUEST Records`
- Table: `sd_my_quest_records`
- Current rows: `0`
- Ownership: server-managed `owner_member_seq`

주요 필드는 World, 제목, 문제, 선택지, 결정, 결정 근거, 근거 URL, 회고, 다음 Quest, 상태, 현재 단계, 시작·완료일, 공개 여부, 정렬 순서입니다.

## API boundary

| Operation | Slug | Member scope |
| --- | --- | ---: |
| List | `my-quest-list` | 1 |
| Get | `my-quest-get` | 1 |
| Create | `my-quest-create` | 1 |
| Update | `my-quest-update` | 1 |
| Delete | `my-quest-delete` | 1 |

- same-origin 회원 세션 사용
- 프런트엔드 API 키 미사용
- `localStorage` 저장 미사용
- 생성 요청에 `is_public=false` 명시
- 공개 포트폴리오 시트와 데이터 혼합 없음

## Published routes

- Main: https://wv1787202495138203.zaemit.ai/
- MY QUEST: https://wv1787202495138203.zaemit.ai/page/my-quest/
- Login: https://wv1787202495138203.zaemit.ai/login
- Sign up: https://wv1787202495138203.zaemit.ai/sign-up
- My page: https://wv1787202495138203.zaemit.ai/my-info

## Verification boundary

비로그인 접근과 로그인 안내는 공개 페이지에서 확인했습니다. 실제 회원 계정이 필요한 생성, 조회, 수정, 완료, 삭제와 회원 간 데이터 격리는 아직 실행 검증하지 않았습니다. 테스트를 위해 가짜 회원 또는 개인 기록을 만들지 않았습니다.
