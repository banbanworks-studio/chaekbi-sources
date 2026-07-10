# 주홍색 연구 원문 출처

- 원저자: Arthur Conan Doyle
- 원제: A Study in Scarlet
- 판본: Project Gutenberg #244 (1887년 초판 계열, "1887년판에서 직접 준비, 오식·구두점까지 원문 그대로 재현" — Transcriber's Note 명시)
- 소스 경로 (표준): `https://raw.githubusercontent.com/GITenberg/A-Study-in-Scarlet_244/master/244.txt` (GITenberg 미러)
- 소스 경로 (예비): Project Gutenberg eBook #244 (gutenberg.org/ebooks/244)
- 판본 검증 마커:
  1. "Produced by Roger Squires" (트랜스크라이버 크레딧, 파일 서두)
  2. "Original Transcriber's Note: This etext is prepared directly from an 1887 edition" (서두 근처)
- 저작권 상태: 퍼블릭 도메인
- 정규화 내역:
  - CRLF → LF (`tr -d '\r'`), PG 라이선스 보일러플레이트(머리말/꼬리말) 제외
  - 제목 페이지("A STUDY IN SCARLET." 표제, 저자명 중복 표기)는 서지 정보이므로 제외하고, 각 Part의 "PART I."/"PART II. _The Country of the Saints._" 헤더부터 본문으로 저장
  - 말미의 "ORIGINAL TRANSCRIBER'S NOTES:"(각주 1~29번, 본문 중 대괄호 각주 번호가 참조하는 원문 이문/오식 주석)는 본문(CHAPTER VII. THE CONCLUSION)에서 참조되는 내용이므로 제외하지 않고 `ch-14.txt` 말미에 그대로 포함
  - Part I(7장) + Part II(7장) = 총 14장, 원문 그대로 무수정
- 파일 단위: `ch-01.txt`~`ch-07.txt` (Part I), `ch-08.txt`~`ch-14.txt` (Part II) — Part 구분은 파일명에 반영하지 않고 이 SOURCE.md에 기록
  - `ch-01.txt` 첫 줄: "PART I." + 부제("Being a reprint from the reminiscences of JOHN H. WATSON, M.D...")
  - `ch-08.txt` 첫 줄: "PART II. _The Country of the Saints._"
  - Part II의 장 번호도 CHAPTER I부터 다시 시작하는 원문 구조 그대로 유지(파일명 `ch-08`~`ch-14`는 연속 번호이지만 각 파일 내부 표제는 "CHAPTER I."~"CHAPTER VII.")
- 비고: Part 경계(ch-07→ch-08)를 놓치기 쉬우니 정규화 스크립트에서 "PART II" 헤더도 챕터 경계로 인식해야 함.
