# 드라큘라 원문 출처

- 원저자: Bram Stoker
- 원제: Dracula
- 판본: Project Gutenberg eBook #345 (단일 판본 — 판본 계열 분기 없음)
- 소스 경로 (표준): `https://raw.githubusercontent.com/GITenberg/Dracula_345/master/345.txt` (GITenberg 미러)
- 소스 경로 (예비): Project Gutenberg eBook #345 (gutenberg.org/ebooks/345)
- 판본 검증 마커:
  1. `paprika hendl` (Chapter I, Jonathan Harker's Journal)
  2. `We want no proofs; we ask none to believe us` (Chapter XXVII, 결말부 Van Helsing 대사)
  - 검증 시 `tr -d '\r' | tr '\n' ' '`로 편 후 grep (하드랩으로 구문이 줄에 걸려 갈라질 수 있음)
- 저작권 상태: 퍼블릭 도메인 (Bram Stoker 1912년 사망, 사후 70년 경과; 원문 자체가 1897년 발표 영어 원본이므로 번역·편집저작권 이슈 없음)
- 정규화 내역:
  - CRLF → LF 개행 정규화 (원본 개행 구조·문단 배치는 그대로 유지, `\r`만 제거)
  - 원문 텍스트 자체는 무수정 (문장·철자·구두점 변경 없음)
  - Project Gutenberg 라이선스 보일러플레이트(머리말/꼬리말) 및 챕터 목차(Table of Contents) 제외, 본문(CHAPTER I~XXVII)만 저장
  - 각 챕터 파일 첫 줄은 원문 그대로의 "CHAPTER 로마숫자" 표제 (2번째 줄에 일지 형식 소제목 — 예: "JONATHAN HARKER'S JOURNAL" — 이 있으면 그것도 원문이므로 그대로 유지)
- 파일 단위: `ch-01.txt` ~ `ch-27.txt` (2자리 zero-pad)
- 비고: 구텐베르크에 축약본·이본 없이 단일 판본만 존재. 표제지(title page)·목차는 원문 서지정보이나 본문이 아니므로 프랑켄슈타인 정규화 표준과 동일하게 제외.
