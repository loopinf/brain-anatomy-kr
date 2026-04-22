# 뇌 구조 학습 · Brain Anatomy (EN · KR · 漢字)

뇌과학 완전 기초. 핵심 15개 부위를 영어·한국어·한자어로 반복 학습할 수 있는 정적 웹사이트입니다. 매일 1분씩 돌려도 금방 입에 붙도록 설계했어요.

## 🧠 핵심 15부위

대뇌피질 4엽 (전두엽·두정엽·측두엽·후두엽), 소뇌, 뇌간(중뇌·교뇌·연수), 간뇌(시상·시상하부), 변연계(해마·편도체), 연결 구조(뇌량), 내분비(뇌하수체).

## 📂 구성

| 페이지 | 용도 |
| --- | --- |
| [`index.html`](index.html) | 전체 모드 랜딩 |
| [`drill.html`](drill.html) | 1초씩 자동 전환되는 드릴. 라운드별로 한글 → 영어 → 한자 순으로 정보가 누적 |
| [`study.html`](study.html) | 클릭 학습 + 플래시카드 + 10문제 퀴즈 |
| [`shorts.html`](shorts.html) | 9:16 세로 프레임 자동 재생. 화면 녹화로 쇼츠 제작 가능 |
| [`script.md`](script.md) | 쇼츠용 5~8초 내레이션 스크립트 15편 |
| [`data.json`](data.json) | 15부위 원본 데이터(영어·한글·한자·위치·기능·어원·암기법) |

## 🚀 로컬에서 보기

```bash
git clone https://github.com/loopinf/brain-anatomy-kr.git
cd brain-anatomy-kr
# 그대로 브라우저로 열거나
open index.html
# 또는 간이 서버
python3 -m http.server 8080
```

## 🌐 GitHub Pages

Settings → Pages → Source: `main` 브랜치 루트를 선택하면 바로 `https://loopinf.github.io/brain-anatomy-kr/`에서 확인됩니다.

## 💡 권장 학습 루틴

1. **아침 1분** — `drill.html` 켜놓고 Round 3까지 한 번 쭉 보기
2. **점심 1분** — `study.html` 플래시카드로 헷갈리는 것만 점검
3. **저녁 1분** — `study.html` 퀴즈 10문제

3일이면 15부위가 영어·한국어·한자어로 자연스럽게 입에 붙습니다.

## 📜 라이선스

MIT
