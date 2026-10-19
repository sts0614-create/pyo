# 중학교 기술·가정 수업실

2022 개정 교육과정 중학교 기술·가정(기술 영역, 성취기준 9기가03·9기가04)의 차시별 수업 자료입니다. 빌드 과정 없이 HTML 파일만으로 작동하는 정적 사이트이며, 역사 수업실 저장소와는 별개입니다.

차시마다 **수업 슬라이드**와 **시뮬레이션**, 단원마다 **학습지**와 **게임**이 있습니다.

## 구조
```
index.html                 첫 화면
tg/index.html              단원 → 차시 → 자료 목록 (성취기준 함께 표시)
tg/<단원>/slidesN.html     N차시 수업 슬라이드
tg/<단원>/sim.html#N       N차시 시뮬레이션
tg/<단원>/worksheet.html   단원 학습지
tg/<단원>/app-*.html       단원 게임
assets/catalog.js          전체 목차와 만들어진 자료(FILES), assets/standards.js 성취기준 문장
tools/                     build_deck.py, build_ws.py, check.py, decks/ (단원별 원본)
```
## 진행 상황
1단원 기술과 기술적 문제 해결, 2단원 발명과 지식재산 완료. 3~7단원은 목록만 있음.
## 새 단원 만들기
`tools/decks/tg_<단원>.py`에 LESSONS, WORKSHEET를 쓰고 `python3 tools/build_deck.py …`, `python3 tools/build_ws.py …` 실행 → sim.html, app-*.html 작성 → `catalog.js` FILES 등록 → `python3 tools/check.py tg`.
## 주의
사진은 아직 없습니다(교사 메모에 사진 자리 표시). 성취기준 문장(standards.js)은 만든 단원 것만 들어 있습니다.
