# 프랑켄슈타인 원문 출처

- 원저자: Mary Shelley
- 원제: Frankenstein; or, The Modern Prometheus
- 판본: 1831년 개정판 계열
- 소스 경로 (표준): `https://raw.githubusercontent.com/GITenberg/Frankenstein_84/master/84.txt` (GITenberg 미러)
- 소스 경로 (예비): Project Gutenberg eBook #84 (gutenberg.org/ebooks/84)
- 판본 검증 마커: 검증 완료 (2026-07-06)
- 저작권 상태: 퍼블릭 도메인
- 정규화 내역:
  - CRLF → LF 개행 정규화 (원본 개행 구조·문단 배치는 그대로 유지, `\r`만 제거)
  - 원문 텍스트 자체는 무수정 (문장·철자·구두점 변경 없음)
  - Letter 1~4(월튼의 편지, 프롤로그)와 Chapter 1~24로 챕터 단위 분할
  - Project Gutenberg 라이선스 보일러플레이트(머리말/꼬리말)는 제외하고 본문만 저장
- 파일 단위: `letter-01.txt` ~ `letter-04.txt` (프롤로그), `ch-01.txt` ~ `ch-24.txt` (본문, 2자리 zero-pad)
- 비고 (이본 문제 등 저본 선정 근거, 해당 시): 프랑켄슈타인은 1818년 초판(익명 출간, 3권 구성, 각 권 챕터 번호 리셋, Milton 인용구 권두 수록, 엘리자베스가 "사촌"으로 서술)과 1831년 개정판(Mary Shelley 실명 출간, 저자 서문 추가, Letter 1~4 뒤 Chapter 1~24로 통합 일련번호, 엘리자베스가 가문에 입양된 "고아"로 서술 변경 등 다수 내용 수정) 두 계열이 별개 텍스트로 유통됨. 본 repo가 채택한 PG#84/GITenberg 84 원문은 "They were fond of the sweet orphan"(엘리자베스=고아 서술) 및 Letter 1~4 뒤 Chapter 1~24 통합 번호 구조를 실제 대조로 확인하여 **1831년 개정판 계열**임을 검증 완료. 1818년 초판(PG#41445 등 별도 계열)은 채택하지 않음 — 혼입 방지 위해 명기.
