# 동물농장 원문 출처

- 소스 유형: **A형 — 영어 원문** (SOURCING.md §2). 파일 단위: **연재형** (§3)
- 원저자: George Orwell (본명 Eric Arthur Blair, 1903–1950)
- 원제: Animal Farm (부제 "A Fairy Story"는 본 저본에 미수록)
- 판본(저본): Project Gutenberg **Australia** eBook No. 0100011, "printed editions which are in the public domain in Australia" 계열 (Producer: Colin Choat, 최초 게시 2001-08 / 최종 갱신 2008-03)
- 소스 경로 (표준): `https://gutenberg.net.au/ebooks01/0100011.txt`
- 소스 경로 (예비): `https://gutenberg.net.au/ebooks01/0100011h.html` (동일 저본 HTML판)
- 저본 선정 근거:
  - **gutenberg.org(미국)에는 본 작품이 없다** — 미국 저작권 존속으로 PG 본토가 수록하지 못함. 따라서 A형 표준(GITenberg/gutenberg.org)이 원천 부재하며, life+50 관할인 호주 PG를 저본으로 채택.
  - 본문은 **10장(Chapter I~X) + 저술일자 "November 1943-February 1944"** 로 구성된 표준 텍스트. 후대에 추가된 "The Freedom of the Press" 서문·우크라이나판 서문은 미수록(대조로 부재 확인) — 저본 계열 혼입 방지 위해 명기.

## 저작권 상태 — ❗관할권 함정 (커밋 전 필수 판단, SOURCING.md §0·§1)

- 🇰🇷 **한국: 퍼블릭 도메인.** 오웰 1950년 사망 → 사후 70년(2020) 만료, 구법 사후 50년(2000)으로도 이미 만료. 1962년 이전 사망이므로 2013년 개정법 소급 없이 만료 확정.
- 🇬🇧🇪🇺🇦🇺🇨🇦 **PD** (life+70 / life+50, 늦어도 2021년~).
- 🇺🇸 **미국: 저작권 존속 (2041년까지).** 1945년 발표작, 발표 후 95년.
- **결정**: 본 repo는 공개 GitHub(미국 호스팅)이다. 한국 각색 파이프라인 기준으로는 PD가 확실하나, **미국 관할 공개배포 리스크를 피하기 위해 오웰 원문 텍스트(`ch-*.txt`)는 커밋하지 않고 로컬 작업 트리에만 둔다.** 루트 `.gitignore`가 `animal-farm/*.txt`를 제외. 이 SOURCE.md(메타데이터·판별 근거, 원문 텍스트 미포함)만 공개 커밋한다.
- 이 결정은 SOURCING.md §0("PD 판별 애매건은 협의, 대화에만 남은 결정은 결정이 아니다")에 따라 여기 기록으로 확정한다. 미국 관할 리스크 재판단 또는 미국 저작권 만료(2041) 시 gitignore 해제 여부를 재검토.
- (참고) 한국어 각색물의 발간·서비스는 원작이 한국 PD이므로 한국 내에서 적법. chaekbi.com이 미국 사용자 대상 서비스·미국 호스팅일 경우 2차적저작물의 미국 노출은 별도 사업 판단 영역 — 원문 소싱과 무관.

## 판본 검증 마커 (하드랩 있음 — 검증 시 `tr -d '\r' | tr '\n' ' '`로 펴서 grep)

1. 오프닝: `had locked the hen-houses for the night, but was too drunk` (ch-01)
2. 클로징: `impossible to say which was which` + 직후 저술일자 `November 1943-February 1944` (ch-10)
3. 개정된 계명이 **대문자로 렌더링**: `ALL ANIMALS ARE EQUAL BUT SOME ANIMALS ARE MORE EQUAL THAN OTHERS` (ch-10) — 소문자 판본과 구별되는 이 저본의 표기 특징
- 검증 완료 (2026-07-14)

## 정규화 내역

- CRLF → LF 개행 정규화 (`\r`만 제거, 원본 개행 구조·문단 배치·하드랩 그대로 유지)
- 원문 텍스트 자체는 무수정 (문장·철자·구두점 변경 없음)
- Chapter I ~ Chapter X 로 챕터 단위 분할, 각 파일 첫 줄은 원문 표제("Chapter I" 등) 그대로
- 책 말미 저술일자 "November 1943-February 1944"는 오웰 원문의 일부이므로 ch-10.txt 끝에 보존
- Project Gutenberg Australia 라이선스 보일러플레이트(머리말/꼬리말)와 편집 추가 "THE END"는 제외하고 본문만 저장

## 파일 단위 상세

- `ch-01.txt` ~ `ch-10.txt` (2자리 zero-pad, 총 10장)
- ⚠️ **위 원문 파일은 gitignore 처리되어 공개 repo에 없다.** 재확보: 표준 경로에서 `curl -sL https://gutenberg.net.au/ebooks01/0100011.txt` 후 위 정규화 재적용.
