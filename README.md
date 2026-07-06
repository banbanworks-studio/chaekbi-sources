# chaekbi-sources

책비(冊秘) 제작 파이프라인에서 사용하는 퍼블릭 도메인 원문 저장소.
판본 검증과 정규화를 마친 상태로 챕터 단위 텍스트 파일을 보관해, 매 제작 세션마다
원문 파싱을 반복하지 않고 필요한 챕터만 바로 받아 쓸 수 있도록 한다.

## Frankenstein (프랑켄슈타인)

- **출처**: Project Gutenberg eBook #84, [GITenberg 미러](https://github.com/GITenberg/Frankenstein_84)
  (`raw.githubusercontent.com/GITenberg/Frankenstein_84/master/84.txt`)
- **판본**: 1831년 개정판 계열
- **저작권**: 퍼블릭 도메인
- **정규화 내역**:
  - CRLF → LF 개행 정규화 (원본 개행 구조·문단 배치는 그대로 유지, `\r`만 제거)
  - 원문 텍스트 자체는 무수정 (문장·철자·구두점 변경 없음)
  - Letter 1~4(월튼의 편지, 프롤로그)와 Chapter 1~24로 챕터 단위 분할
  - Project Gutenberg 라이선스 보일러플레이트(머리말/꼬리말)는 제외하고 본문만 저장

### 파일 구조

```
frankenstein/
  letter-01.txt ~ letter-04.txt   # 월튼의 편지 (프롤로그)
  ch-01.txt ~ ch-24.txt           # 본문 챕터 (2자리 zero-pad)
pg84.txt                          # 원문 전체 (CRLF 정규화만 적용, 미분할)
```

### 접근 예시

```
https://raw.githubusercontent.com/banbanworks-studio/chaekbi-sources/main/frankenstein/ch-12.txt
```
