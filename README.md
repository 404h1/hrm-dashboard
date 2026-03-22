# HRM Dashboard

> Meta Llama Academy 인적자원 관리 시스템 프로토타입

직원의 역량을 추적하고, 업무 보고를 관리하며, 개인 성장을 지원하는 Flask 기반 HRM 대시보드입니다.

## 개요

단순한 프로젝트 관리 도구를 넘어, 조직 내 인원의 **강점 파악 → 프로젝트 배정 → 업무 보고 → 역량 개발**로 이어지는 인적자원 관리 흐름을 하나의 화면에서 처리할 수 있도록 설계되었습니다.

## 주요 기능

### 인력 관리
- 직원 프로필 및 강점(Strengths) 데이터 관리
- 프로젝트별 담당 인원 배정 및 태스크 현황 조회

### 업무 보고
- **일간 보고서** — 날짜별 업무 내역 작성 및 수정
- **주간 보고서** — 주 단위 업무 요약
- **월간 보고서** — 월별 성과 정리 및 캘린더 시각화

### 역량 개발
- 직원 강점 기반 **교육 콘텐츠 자동 추천**
- 개인 역량과 연결된 성장 경로 제안

### 일정 관리
- 오전 / 오후 단위 업무 일정 등록 및 조회

## 기술 스택

| 분류 | 기술 |
|------|------|
| Backend | Python 3, Flask |
| Frontend | HTML, CSS, JavaScript |
| Data Store | JSON |

## 시작하기

```bash
# 레포지토리 클론
git clone https://github.com/404h1/hrm-dashboard.git
cd hrm-dashboard/project_dashboard

# 의존성 설치
pip install -r requirements.txt

# 서버 실행
python app.py
```

`http://localhost:5000` 에서 확인

## 프로젝트 구조

```
project_dashboard/
├── app.py                        # Flask 앱 진입점
├── requirements.txt
├── data/                         # JSON 데이터 저장소
│   ├── users.json                # 직원 프로필 및 강점
│   ├── projects.json             # 프로젝트 및 태스크
│   ├── schedules.json            # 일정
│   ├── daily_reports.json        # 일간 보고서
│   ├── weekly_reports.json       # 주간 보고서
│   ├── monthly_reports.json      # 월간 보고서
│   └── education_recommendations.json  # 교육 추천
├── static/
│   ├── css/style.css
│   └── js/script.js
└── templates/
    ├── layout.html
    ├── index.html                # 메인 대시보드
    └── project_detail.html       # 프로젝트 상세
```