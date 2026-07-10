# 레미제라블 (Les Misérables) 원문 출처

- 소스 유형: B형 (비영어 서양 고전) — 번역 저본이 아닌 **원어(프랑스어) 원문 저본** 케이스.
  ※ B형 원어저본 하위분기 명문화는 성경 확정 대기(커밋 비차단).
- 원저자 / 원제: Victor Hugo (1802–1885) / Les Misérables (초판 1862)
- 판본(저본): fr.wikisource "Les Misérables (1908)", Ollendorff / Imprimerie nationale,
  Œuvres complètes 계열, texte établi par Gustave Simon (1851–1926).
- 저본 선정 근거: Œuvres complètes 정본 계열 학술 표준. 편집자 Simon 사후 70년(1996) 만료로 편집저작권까지 클리어.
- 소스 경로(표준): fr.wikisource.org "Les Misérables (1908)/Tome N/Livre M/장" leaf,
  API `action=parse&prop=text` 렌더 추출. 예비: archive.org PD 스캔.
- 저본 djvu (fr.wikisource ProofreadPage index, Œuvres complètes, Impr. nat., 계열 *Roman*):
  - Tome 1 (Fantine) ← `Hugo - Œuvres complètes, Impr. nat., Roman, tome III.djvu`
  - Tome 2 (Cosette) ← `Hugo - Œuvres complètes, Impr. nat., Roman, tome IV.djvu`
  - Tome 3 (Marius) ← `Hugo - Œuvres complètes, Impr. nat., Roman, tome IV.djvu` (Tome 2와 동일 물리 권)
  - Tome 4 (L'idylle rue Plumet…) ← `Hugo - Œuvres complètes, Impr. nat., Roman, tome V.djvu`
  - Tome 5 (Jean Valjean) ← `Hugo - Œuvres complètes, Impr. nat., Roman, tome VI.djvu`
- 판본 검증 마커: (검증 완료 2026-07-09, `tr -d '\r' | tr '\n' ' '` 후 grep)
  - ① 서문(preface.txt): `Tant qu'il existera, par le fait des lois et des mœurs`
  - ② 팡틴 1권 1장(ch-001.txt): `En 1815, M. Charles-François-Bienvenu Myriel était évêque de Digne`
  - ③ (추가) 최종장(ch-365.txt) 묘비명: `Il dort. Quoique le sort fût pour lui bien étrange` …
    말미 `Comme la nuit se fait lorsque le jour s'en va.`
- 저작권 상태(커밋 텍스트 기준): 원작 사후 70년(1955)·편집자 Simon 사후 70년(1996) 모두 만료 → PD.
  fr.wikisource CC BY-SA는 전사·조판 기여에 적용, 본문(위고 원문)은 PD이므로 원문 저장에 제약 없음.
- 정규화: CRLF→LF, BOM 없음, UTF-8. 보일러플레이트(네비·페이지번호·편집각주·헤더템플릿·references) 제외.
  렌더 추출이라 인쇄본 intra-문단 하드랩 재현 불가 → 1문단 1행. 문단 경계는 빈 줄 1개, 본문 무수정.
- 파일 단위: `preface.txt` + `ch-001.txt` ~ `ch-365.txt` (3자리 — 章 규모 때문에 가이드 2자리 규칙 확장).

## 목차 (ch-NNN ↔ 部(Tome)/卷(Livre)/章)

章은 部→卷→章 순으로 빈틈없이 연속 배열됨(구조적 정렬 = fr.wikisource Tome-index 링크 순과 바이트 단위 일치 검증). 아래는 卷 단위 파일 범위 — 연속 배열이므로 이 표로 ch-NNN ↔ 章 대응이 완전 결정됨.

| 部 (Tome) | 卷 (Livre) | ch 파일 범위 | 章수 |
|---|---|---|---|
| 1 · Fantine | Livre 1 | ch-001–ch-014 | 14 |
| 1 · Fantine | Livre 2 | ch-015–ch-027 | 13 |
| 1 · Fantine | Livre 3 | ch-028–ch-036 | 9 |
| 1 · Fantine | Livre 4 | ch-037–ch-039 | 3 |
| 1 · Fantine | Livre 5 | ch-040–ch-052 | 13 |
| 1 · Fantine | Livre 6 | ch-053–ch-054 | 2 |
| 1 · Fantine | Livre 7 | ch-055–ch-065 | 11 |
| 1 · Fantine | Livre 8 | ch-066–ch-070 | 5 |
| 2 · Cosette | Livre 1 | ch-071–ch-089 | 19 |
| 2 · Cosette | Livre 2 | ch-090–ch-092 | 3 |
| 2 · Cosette | Livre 3 | ch-093–ch-103 | 11 |
| 2 · Cosette | Livre 4 | ch-104–ch-108 | 5 |
| 2 · Cosette | Livre 5 | ch-109–ch-118 | 10 |
| 2 · Cosette | Livre 6 | ch-119–ch-129 | 11 |
| 2 · Cosette | Livre 7 | ch-130–ch-137 | 8 |
| 2 · Cosette | Livre 8 | ch-138–ch-146 | 9 |
| 3 · Marius | Livre 1 | ch-147–ch-159 | 13 |
| 3 · Marius | Livre 2 | ch-160–ch-167 | 8 |
| 3 · Marius | Livre 3 | ch-168–ch-175 | 8 |
| 3 · Marius | Livre 4 | ch-176–ch-181 | 6 |
| 3 · Marius | Livre 5 | ch-182–ch-187 | 6 |
| 3 · Marius | Livre 6 | ch-188–ch-196 | 9 |
| 3 · Marius | Livre 7 | ch-197–ch-200 | 4 |
| 3 · Marius | Livre 8 | ch-201–ch-222 | 22 |
| 4 · L'idylle rue Plumet… | Livre 1 | ch-223–ch-228 | 6 |
| 4 · L'idylle rue Plumet… | Livre 2 | ch-229–ch-232 | 4 |
| 4 · L'idylle rue Plumet… | Livre 3 | ch-233–ch-240 | 8 |
| 4 · L'idylle rue Plumet… | Livre 4 | ch-241–ch-242 | 2 |
| 4 · L'idylle rue Plumet… | Livre 5 | ch-243–ch-248 | 6 |
| 4 · L'idylle rue Plumet… | Livre 6 | ch-249–ch-251 | 3 |
| 4 · L'idylle rue Plumet… | Livre 7 | ch-252–ch-255 | 4 |
| 4 · L'idylle rue Plumet… | Livre 8 | ch-256–ch-262 | 7 |
| 4 · L'idylle rue Plumet… | Livre 9 | ch-263–ch-265 | 3 |
| 4 · L'idylle rue Plumet… | Livre 10 | ch-266–ch-270 | 5 |
| 4 · L'idylle rue Plumet… | Livre 11 | ch-271–ch-276 | 6 |
| 4 · L'idylle rue Plumet… | Livre 12 | ch-277–ch-284 | 8 |
| 4 · L'idylle rue Plumet… | Livre 13 | ch-285–ch-287 | 3 |
| 4 · L'idylle rue Plumet… | Livre 14 | ch-288–ch-294 | 7 |
| 4 · L'idylle rue Plumet… | Livre 15 | ch-295–ch-298 | 4 |
| 5 · Jean Valjean | Livre 1 | ch-299–ch-322 | 24 |
| 5 · Jean Valjean | Livre 2 | ch-323–ch-328 | 6 |
| 5 · Jean Valjean | Livre 3 | ch-329–ch-340 | 12 |
| 5 · Jean Valjean | Livre 4 | ch-341–ch-341 | 1 |
| 5 · Jean Valjean | Livre 5 | ch-342–ch-349 | 8 |
| 5 · Jean Valjean | Livre 6 | ch-350–ch-353 | 4 |
| 5 · Jean Valjean | Livre 7 | ch-354–ch-355 | 2 |
| 5 · Jean Valjean | Livre 8 | ch-356–ch-359 | 4 |
| 5 · Jean Valjean | Livre 9 | ch-360–ch-365 | 6 |

- 部 5개 / 卷 48개(8+8+8+15+9) / 章 365개 — 통행본 표준 구성과 일치.
- Tome 5/Livre 4("Javert déraillé")는 하위 `/NN` 없이 卷 페이지에 본문이 직접 실린 **단일 章 권** → 구조 정렬 시 章 0으로 처리해 ch-341에 제자리 배치.

## 비고

- 章 총수: **365** (preface.txt 별도). 部 5 · 卷 48.
- 저본 소스 단위: fr.wikisource 콘텐츠 leaf(`Tome N/Livre M/장`)를 API 렌더(`prop=text`)로 추출.
  실제 본문은 ProofreadPage `Page:…djvu/NN`(스캔 저본)에서 `<pages index=… />`로 transclude됨.
  **Page:djvu 직접 순회는 章 경계와 페이지 경계 불일치로 배제**, 章 무결성 위해 콘텐츠 leaf 단위 채택.
- 수록에서 제외한 fr.wikisource 페이지 2건 (둘 다 다른 곳에 보존된 텍스트의 **바이트 단위 중복본**이라 원문 유실 없음):
  - `Les Misérables (1908)/Tome 5//Livre 5/05` — 슬래시 중복 오식 페이지, 정상 `Tome 5/Livre 5/05`(= ch-346)와 바이트 동일.
  - `Les Misérables (1908)/Tome 1/Livre 1/00` — 권두 에피그래프("Tant qu'il existera…"), `preface.txt`와 동일 → 본문 章 시퀀스에서 제외하고 preface.txt로만 보존.
- 각 파일 첫 행은 원문 章 표제(로마숫자 표제 형식, 예: `I` / `II`).
