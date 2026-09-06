# 스킨어스 SKINEARTH
<img src="../assets/main.png" width="auto"/>


## 🌍 ABOUT SKINEARTH

### 프로젝트 한 줄 소개

> 내 피부에도 기후가 있다 — 생활 환경과 피부 컨디션의 숨은 인과관계를 발견하는 AI 기록 서비스
> 

### 개발 배경 / 문제 정의

잡코리아 설문에 따르면 겨울철 사무실 환경에 불편을 느끼는 직장인은 75.1%에 달했고, 그중 63.6%는 건조한 사무실 때문에 피부가 건조해지는 문제를 가장 큰 고민으로 꼽았습니다. 냉난방 환경이 이미 사무직 직장인들의 피부 트러블 원인으로 인식되고 있다는 뜻입니다.

그러나 우리는 냉난방, 스크린타임, 수면 같은 일상 변수가 실제로 내 피부에 어떤 영향을 주는지 데이터로 확인해본 적이 없습니다. 기존 스킨케어 서비스 역시 피부 상태를 진단하고 제품을 추천하는 데 그칠 뿐, 사용자 주변 환경에서 원인을 찾아 결과와 연결해주지는 못했습니다.

SKINEARTH는 피부를 하나의 작은 행성으로, 반복되는 트러블 문제를 그 행성의 기후 문제로 바라봅니다. 지구온난화의 원인을 개인이 완전히 통제할 수 없듯, 피부 문제의 원인도 완전히 없애기는 어렵습니다. 그래서 원인을 없애주겠다고 약속하는 대신, 사용자가 스스로 원인을 규명하고 그에 맞는 완화·적응 전략을 찾아가도록 돕습니다.

### 프로젝트 목표

- **진단이 아닌 원인 규명**: 피부 상태 판정이나 제품 추천이 아니라, 일상 환경 변수와 피부 컨디션 사이의 인과관계를 데이터로 밝혀냅니다.
- **개인화된 원인 발견**: 모든 사용자에게 같은 원인을 알려주는 것이 아니라, 변수별 독립 분석을 통해 개인마다 실제 영향력이 큰 원인 1~2개를 자동으로 찾아냅니다.
- **콜드스타트 없는 개인화**: 기록이 없는 신규 사용자에게도 첫날부터 추정 예보를 제공하고, 기록이 쌓일수록 자동으로 데이터 기반 예보로 정교해집니다.
- **부담 없는 습관 형성**: 하루 15초의 기록과 최소 단위의 게이미피케이션(스트릭, 레벨업)으로 지속 가능한 기록 습관을 만듭니다.

## 📖 OVERVIEW

### 핵심 기능

| 기능 | 설명 |
| --- | --- |
| **궤도<br> 관측<br> 로그** | 냉난방·스크린타임·수면·스트레스·식사 규칙성 5가지 환경 변수와 오늘의 피부 컨디션을 하루 15초, 원탭으로 기록 |
| **행성 <br> 온도계** | 누적 기록을 하나의 직관적인 지표로 압축해, 내 피부가 안정 궤도에서 얼마나 벗어나 있는지 시각화 |
| **내일의 <br>궤도<br>예보** | 통계 엔진이 계산한 개인별 상관관계를 바탕으로 위험도 점수와 주요 원인을 예측하고, 생성형 AI가 자연어 코멘트로 설명. 기록이 적은 초기에는 프로필 기반 추정치로, 데이터가 쌓이면 자동으로 데이터 기반 결과로 전환 |
| **탐사<br> 미션** | 오늘의 주요 원인에 맞춘 행동 미션을 제안. 사전 정의된 카테고리·행동 슬롯 안에서 AI가 상황에 맞는 조합을 선택해 개인화된 문구로 전달 |
| **궤도 <br>히스토리** | 주/월 단위로 온난화 지수 추이, 주요 원인 변화, 미션 이행률을 확인 |

### 사용자 이용 흐름

```
온보딩
 └ 서비스 소개 → 로그인/약관 동의 → 개인화 설문(닉네임/상태/피부고민)
      │
      ▼
홈 (행성 온도계 + 오늘의 예보 요약)
      │
      ├─▶ 궤도 관측 로그 (하루 15초 기록)
      │        │
      │        └─▶ 유효기록 10건 미만: 추정 예보 (프로필 기반)
      │             유효기록 10건 이상: 데이터 기반 예보로 자동 전환
      │
      ├─▶ 내일의 궤도 예보 (위험도 · 주요 원인 · AI 코멘트)
      │        │
      │        └─▶ 탐사 미션 (원인 맞춤 행동 제안)
      │
      └─▶ 궤도 히스토리 (장기 추이 확인)
```

### 주요 화면

| 화면 | 설명 |
| --- | --- |
| 온보딩 | 서비스 소개, 로그인/회원가입, 개인화 설문, 첫 기록 유도 |
| 홈 | 행성 온도계, 오늘 기록 상태, 예보 요약, 오늘의 미션 바로가기 |
| 궤도 관측 로그 | 일일 기록 입력 화면 |
| 내일의 궤도 예보 | 내일 변수 입력 및 예보 결과 화면 |
| 탐사 미션 | 미션 카드 및 상호작용(다른 미션 보기 / 더 쉬운 미션으로 / 이 카테고리 그만 보기) |
| 궤도 히스토리 | 추이 그래프, 원인 변화 타임라인, 미션 이행률, 뱃지 |
| 마이페이지 | 계정 정보, 프로필 수정, 데이터 초기화, 알림 설정 |

## 👤 Members
| PM | FE | FE | BE | BE |
| :---: | :---: | :---: | :---: | :---: |
| <img src="../assets/박수현.jpg" width="100"/> | <img src="../assets/박서현.jpg" width="100"/> | <img src="../assets/박영서.jpg" width="100"/> | <img src="../assets//강지윤.jpg" width="100"/> | <img src="이미지주소6" width="100"/> |
| 박수현 | 박서현 | 박영서 | 강지윤 | 박수빈 |
| 서비스 기획 (PRD)<br>기능명세서 · IA<br>Wireframe<br>디자인 시스템 · UI 디자인<br>IR Deck | 로그인 페이지<br>회원가입 페이지<br>온보딩 페이지<br>홈 페이지<br>히스토리 페이지 | 스플래시 페이지<br>기록 페이지<br>예보 페이지<br>미션 페이지<br>마이페이지 | 예보 통계<br>AI 예보 코멘트<br>AI 미션 생성<br>원인 타임라인<br>뱃지<br>배포 | 로그인·회원가입<br>온보딩 설문<br>일일 기록<br>홈<br>히스토리<br>마이페이지 |

## 🛠 TECH STACK
<h3 align="center">Frontend</h3>

<p align="center">
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=000000">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=000000">
  <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=FFFFFF">
  <br/>
  <img src="https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=FFFFFF">
</p>

<h3 align="center">Backend</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Java_21-007396?style=for-the-badge&logo=openjdk&logoColor=FFFFFF">
  <img src="https://img.shields.io/badge/Spring_Boot_4.1.0-6DB33F?style=for-the-badge&logo=springboot&logoColor=FFFFFF">
  <img src="https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=FFFFFF">
  <br/>
  <img src="https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=gradle&logoColor=FFFFFF">
</p>

<h3 align="center">AI</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=FFFFFF">
</p>

<h3 align="center">Database</h3>

<p align="center">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=FFFFFF">
</p>

<h3 align="center">Infra / Deployment</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=FFFFFF">
  <img src="https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=FFFFFF">
</p>

<h3 align="center">Tools</h3>

<p align="center">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=FFFFFF">
  <img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=FFFFFF">
  <img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=FFFFFF">
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=000000">
</p>

## 🚀 DEPLOYMENT
### Service URL

> SKINEARTH<br>
> https://skinearth.vercel.app 

## 📚 WORKSPACE

- 📝 **Notion** — [SKINEARTH Workspace](https://daisy-licorice-73f.notion.site/likelion-skinearth?pvs=74)
- 📑 **Swagger** — [SKINEARTH API Documentation](https://skinearth-api.up.railway.app/swagger-ui/index.html#/)
- 🎨 **Figma** — [SKINEARTH Figma Design](https://www.figma.com/files/team/1631929564551131955/folder/631111401?fuid=1458373486563603398)
