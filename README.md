# 🦙 Llama Academy Dashboard

Meta Llama Academy 프로젝트 관리 대시보드 — Flask 기반 개인 업무 관리 웹 애플리케이션

## 주요 기능

- **프로젝트 관리** — 담당 프로젝트 현황 및 태스크 확인
- **일정 관리** — 오전/오후 일정 등록 및 조회
- **업무 보고서** — 일간 / 주간 / 월간 보고서 작성 및 조회
- **교육 추천** — 강점 기반 교육 콘텐츠 추천
- **캘린더** — 월별 보고서 작성 현황 시각화

## 기술 스택

| 분류 | 기술 |
|------|------|
| Backend | Python, Flask |
| Frontend | HTML, CSS, JavaScript |
| Data | JSON |

## 시작하기

```bash
# 1. 레포지토리 클론
git clone https://github.com/404h1/llama-academy-dashboard.git
cd llama-academy-dashboard/project_dashboard

# 2. 의존성 설치
pip install -r requirements.txt

# 3. 실행
python app.py
```

브라우저에서 `http://localhost:5000` 접속

## 프로젝트 구조

```
project_dashboard/
├── app.py                  # Flask 애플리케이션
├── requirements.txt
├── data/                   # JSON 데이터
│   ├── users.json
│   ├── projects.json
│   ├── schedules.json
│   ├── daily_reports.json
│   ├── weekly_reports.json
│   ├── monthly_reports.json
│   └── education_recommendations.json
├── static/
│   ├── css/style.css
│   └── js/script.js
└── templates/
    ├── layout.html
    ├── index.html
    └── project_detail.html
```
