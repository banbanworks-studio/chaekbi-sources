# chaekbi-sources

책비(冊秘) 제작 파이프라인에서 사용하는 퍼블릭 도메인 원문 저장소.

이 repo의 모든 텍스트는 퍼블릭 도메인 원문이며, 정규화(개행 정리·챕터 분할) 외
내용 수정이 없다. 책비(chaekbi.com)의 각색 저작물과는 별개다.

## 구조

- 폴더 하나 = 작품 하나.
- 각 작품 폴더 안의 `SOURCE.md`가 그 작품의 출처·판본·저본 선정 근거를 기록한다.
  원문 텍스트를 가져오거나 재검증할 때는 반드시 해당 작품의 `SOURCE.md`를 먼저 확인한다.
- 뿌리/장르/줄기 등 편집 지침(각색 가이드)은 이 repo의 대상이 아니다. 여기에는
  정규화된 원문만 둔다.

## 파일 단위 원칙

규칙 원본은 [SOURCING.md](SOURCING.md) §3.

## 작품 목록

| 폴더 | 작품 | 유형 |
|---|---|---|
| [frankenstein/](frankenstein/) | 프랑켄슈타인 | 연재형 |
| [pride-and-prejudice/](pride-and-prejudice/) | 오만과 편견 | 연재형 |
| [count-of-monte-cristo/](count-of-monte-cristo/) | 몬테크리스토 백작 | 연재형 |
| [honggildong/](honggildong/) | 홍길동전 | 연재형 |
| [dracula/](dracula/) | 드라큘라 | 연재형 |
| [sherlock-holmes-casebook/](sherlock-holmes-casebook/) | 셜록 홈즈 전집 (장편 4 + 단편집 5, 폴더별 SOURCE.md 참조) | 연재형/옴니버스 혼재 |
| [liaozhai/](liaozhai/) | 요재지이 | 옴니버스 |
| [ugetsu-monogatari/](ugetsu-monogatari/) | 우게츠 이야기 | 옴니버스 |
| [samguk-yusa/](samguk-yusa/) | 삼국유사 | 옴니버스 |
| [kim-yujeong-anthology/](kim-yujeong-anthology/) | 김유정 단편집 | 옴니버스 |
| [korean-modern-anthology/](korean-modern-anthology/) | 원문 서고(근대 단편 20편) | 단편형(원문 그대로) |
| [jeonuchi-jeon/](jeonuchi-jeon/) | 전운치전 | 연재형(단일 회차) |
| [animal-farm/](animal-farm/) | 동물농장 | 연재형 (원문 `ch-*.txt`는 미국 관할 저작권으로 gitignore·로컬 전용, SOURCE.md만 공개) |
