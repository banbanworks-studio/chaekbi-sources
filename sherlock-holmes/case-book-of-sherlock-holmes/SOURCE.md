# 셜록 홈즈의 사건집 원문 출처

- 원저자: Arthur Conan Doyle
- 원제: The Case-Book of Sherlock Holmes (12편 단편집, 1927)
- 판본: Project Gutenberg #69700 (단일 판본 — 판본 계열 분기 없음. 파일명이 `69700-0.txt`인 점 주의, 다른 판본은 `{ID}.txt`)
- 소스 경로 (표준): `https://raw.githubusercontent.com/GITenberg/The-case-book-of-Sherlock-Holmes_69700/master/69700-0.txt` (GITenberg 미러)
- 소스 경로 (예비): Project Gutenberg eBook #69700 (gutenberg.org/ebooks/69700)
- 판본 검증 마커: 검증 완료 (2026-07-07)
  1. "Produced by: Al Haines" (트랜스크라이버 크레딧)
  2. "*** START OF THE PROJECT GUTENBERG EBOOK THE CASE-BOOK OF SHERLOCK HOLMES ***" (시작 마커, 2줄에 걸쳐 표기됨)
  3. CONTENTS 목차의 12편 제목과 본문 표제(로마 숫자 + 대문자 제목) 순서·자구 일치 확인
- 저작권 상태: 퍼블릭 도메인
- 정규화 내역:
  - CRLF → LF (`\r`만 제거, 원본 개행 구조·문단 배치는 그대로 유지)
  - 원문 텍스트 자체는 무수정 (문장·철자·구두점 변경 없음)
  - Project Gutenberg 라이선스 보일러플레이트(머리말/꼬리말) 제외
  - 저자 서문(PREFACE, "I fear that Mr. Sherlock Holmes may become..."로 시작)과 CONTENTS(목차)는 12편 스토리 본문이 아니므로 제외 — 별도 파일로 저장하지 않음
  - 말미의 저자 저서 목록 광고면("By A. Conan Doyle" 이하 도서 목록)과 인쇄소 소개("Printed in Great Britain by Butler & Tanner Ltd., Frome and London")는 본문이 아니므로 제외
  - 본문(로마 숫자 표제 I~XII)만 12편 개별 파일로 분할
- 파일 단위 (수록 순서):
  1. tale-01.txt 저명한 의뢰인 (The Adventure of the Illustrious Client)
  2. tale-02.txt 창백한 병사 (The Adventure of the Blanched Soldier)
  3. tale-03.txt 마자랭 보석 (The Adventure of the Mazarin Stone)
  4. tale-04.txt 세 박공의 집 (The Adventure of the Three Gables)
  5. tale-05.txt 서식스의 흡혈귀 (The Adventure of the Sussex Vampire)
  6. tale-06.txt 세 명의 개리뎁 (The Adventure of the Three Garridebs)
  7. tale-07.txt 토르교 사건 (The Problem of Thor Bridge)
  8. tale-08.txt 기어다니는 남자 (The Adventure of the Creeping Man)
  9. tale-09.txt 사자의 갈기 (The Adventure of the Lion's Mane)
  10. tale-10.txt 베일 쓴 하숙인 (The Adventure of the Veiled Lodger)
  11. tale-11.txt 쇼스컴 관 (The Adventure of Shoscombe Old Place)
  12. tale-12.txt 은퇴한 물감 제조업자 (The Adventure of the Retired Colourman)
- 비고: 이 판본은 각 편 표제가 "로마 숫자(단독 줄) + 빈 줄 + 대문자 제목(단독 줄)" 2줄 구조로 되어 있어, 한 줄에 붙어 있는 다른 폴더(예: adventures-of-sherlock-holmes의 "ADVENTURE II. THE RED-HEADED LEAGUE")와 원문 자체의 조판 방식이 다름. 임의로 한 줄에 합치지 않고 원문 그대로 로마 숫자를 각 파일의 첫 줄로 유지함. 서문·목차·말미 광고면 제외 판단에 이견이 있으면 커밋 보류하고 확인 요망.
