# ThinkPM - Thinking Project Manager

<div align="center">
  <img src="https://i.ibb.co/pLH3WhQ/favicon.png" alt="ThinkPM Logo" width="120"/>
  
  ### 프로젝트 포트폴리오 웹사이트
  
  [![Netlify](https://img.shields.io/badge/Deployed%20on-Netlify-00C7B7?style=flat-square&logo=netlify)](https://netlify.com)
  [![React](https://img.shields.io/badge/React-18.3.1-61DAFB?style=flat-square&logo=react)](https://reactjs.org/)
  [![TypeScript](https://img.shields.io/badge/TypeScript-5.5.3-3178C6?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
  [![Vite](https://img.shields.io/badge/Vite-5.4.2-646CFF?style=flat-square&logo=vite)](https://vitejs.dev/)
  
  [🌐 Live Demo](#) | [📧 Contact](mailto:your-email@example.com)
</div>

---

## 📋 목차

- [소개](#-소개)
- [주요 기능](#-주요-기능)
- [기술 스택](#-기술-스택)
- [프로젝트 구조](#-프로젝트-구조)
- [시작하기](#-시작하기)
- [포트폴리오 프로젝트](#-포트폴리오-프로젝트)
- [다국어 지원](#-다국어-지원)
- [테마 시스템](#-테마-시스템)
- [배포](#-배포)
- [라이선스](#-라이선스)

---

## 🎯 소개

**ThinkPM**은 프로젝트 매니저이자 개발자인 **홍평강(Pyungkang Hong)**의 포트폴리오 웹사이트입니다. 

이 사이트는 10개 이상의 실제 프로젝트 경험을 효과적으로 보여주며, 각 프로젝트의 세부 사항, 팀 구성, 기술 스택, 그리고 성과 지표를 직관적으로 제공합니다.

### 💡 왜 ThinkPM인가?

- **실용주의적 접근**: 복잡한 문제를 간단하고 효율적인 솔루션으로 해결
- **다양한 경험**: 웹, 앱, ERP, CRM, 헬스케어, 핀테크 등 다양한 도메인 경험
- **자동화 전문가**: n8n, Python을 활용한 워크플로우 자동화 및 최적화

---

## ✨ 주요 기능

### 🎨 **반응형 디자인**
- 모바일, 태블릿, 데스크톱 모든 디바이스에서 완벽하게 작동
- 유연한 그리드 레이아웃과 부드러운 애니메이션

### 🌓 **다크 모드**
- 사용자 선호도에 따라 라이트/다크 테마 전환
- 로컬 스토리지를 통한 설정 저장

### 🌍 **다국어 지원 (i18n)**
- 한국어 (KR) / 영어 (EN) 완벽 지원
- 모든 프로젝트 설명, UI 텍스트 다국어화
- 실시간 언어 전환

### 📱 **프로젝트 필터링**
- 프로젝트 타입별 필터링 (전체 / 웹 / 앱)
- 직관적인 토글 UI

### 🔍 **상세 프로젝트 페이지**
- 각 프로젝트별 독립된 상세 페이지
- 스크린샷 갤러리
- 팀 구성원 정보
- 기술 스택 배지
- 성과 지표 시각화
- 관련 링크 (Live, GitHub, Notion, Figma 등)

### 👤 **프로필 페이지**
- 개발자 소개
- 경력 사항
- 기술 스택
- 연락처 정보

---

## 🛠 기술 스택

### **Frontend**
- **React 18.3.1** - UI 라이브러리
- **TypeScript 5.5.3** - 타입 안정성
- **React Router DOM 6.22.3** - 클라이언트 사이드 라우팅
- **Vite 5.4.2** - 빠른 빌드 도구 및 개발 서버

### **스타일링**
- **Tailwind CSS 3.4.1** - 유틸리티 기반 CSS 프레임워크
- **PostCSS 8.4.35** - CSS 변환 도구
- **Autoprefixer 10.4.18** - 자동 CSS 벤더 프리픽스

### **국제화 (i18n)**
- **i18next 23.10.1** - 국제화 프레임워크
- **react-i18next 14.1.0** - React용 i18next 바인딩

### **UI/UX**
- **lucide-react 0.344.0** - 아이콘 라이브러리

### **개발 도구**
- **ESLint 9.9.1** - 코드 품질 도구
- **TypeScript ESLint 8.3.0** - TypeScript용 ESLint 규칙

---

## 📁 프로젝트 구조

```
PK_portfolio/
├── public/                     # 정적 파일
├── src/
│   ├── components/            # React 컴포넌트
│   │   ├── Header.tsx         # 헤더 (테마, 언어, 프로필)
│   │   ├── ProjectCard.tsx    # 프로젝트 카드
│   │   ├── ProjectDetail.tsx  # 프로젝트 상세 페이지
│   │   ├── ProjectGrid.tsx    # 프로젝트 그리드 레이아웃
│   │   ├── ProjectSection.tsx # 프로젝트 섹션 컨테이너
│   │   ├── ProjectToggle.tsx  # 프로젝트 타입 필터
│   │   └── Profile/           # 프로필 관련 컴포넌트
│   │       ├── ProfilePage.tsx
│   │       └── ...
│   ├── data/
│   │   └── projects.ts        # 프로젝트 데이터 (10개 프로젝트)
│   ├── hooks/
│   │   ├── useTheme.ts        # 테마 관리 훅
│   │   └── useProjectFilter.ts # 프로젝트 필터 훅
│   ├── i18n/
│   │   ├── index.ts           # i18n 설정
│   │   └── locales/           # 번역 파일
│   │       ├── en.json        # 영어 번역
│   │       └── kr.json        # 한국어 번역
│   ├── types/
│   │   └── index.ts           # TypeScript 타입 정의
│   ├── App.tsx                # 메인 앱 컴포넌트
│   ├── main.tsx               # 진입점
│   └── index.css              # 전역 스타일
├── index.html                 # HTML 템플릿
├── package.json               # 의존성 관리
├── tsconfig.json              # TypeScript 설정
├── tailwind.config.js         # Tailwind CSS 설정
├── vite.config.ts             # Vite 설정
├── netlify.toml               # Netlify 배포 설정
└── README.md                  # 프로젝트 문서
```

---

## 🚀 시작하기

### **필수 조건**
- Node.js 18.x 이상
- npm 또는 yarn

### **설치**

```bash
# 저장소 클론
git clone https://github.com/PyungkangHong094/PK_portfolio.git

# 디렉토리 이동
cd PK_portfolio

# 의존성 설치
npm install
```

### **개발 서버 실행**

```bash
npm run dev
```

개발 서버가 `http://localhost:5173`에서 실행됩니다.

### **프로덕션 빌드**

```bash
npm run build
```

빌드된 파일은 `dist/` 디렉토리에 생성됩니다.

### **프로덕션 미리보기**

```bash
npm run preview
```

### **린트 검사**

```bash
npm run lint
```

---

## 💼 포트폴리오 프로젝트

이 포트폴리오는 다음과 같은 **10개의 실제 프로젝트**를 포함하고 있습니다:

### 1. **D2 Design and Works** (2022.11 - 2024.01)
- **유형**: 웹 플랫폼
- **설명**: 욕실 인테리어 디자인 관리를 위한 종합 ERP 시스템
- **기술**: n8n, Python, VM Server, Notion
- **역할**: 프리랜서 개발 컨설턴트

### 2. **3TP Trading Strategy** (2022.03 - 2022.11)
![3TP Trading Strategy Screen](/public/images/3tp-strategy.png)
- **유형**: 웹 플랫폼
- **설명**: Pine Script를 활용한 고급 트레이딩 전략 개발 및 자동화
- **기술**: Pine Script, Python, TradingView API, VM Server
- **역할**: 단독 프로젝트

### 3. **ChartQ** (2024.05 - 현재)
- **유형**: 모바일 앱
- **설명**: 금융 차트 학습 앱: 퀴즈, 게임 및 트레이딩 전략 제공
- **기술**: Flutter, Supabase, Pine Script, Python, SQLite/Hive
- **역할**: 프로젝트 매니저
- **팀**: 4명 (PM, AI 개발자, 백엔드, UI/UX)
- **링크**: [chartq.app](https://chartq.app/)

### 4. **Fidesbankcard** (2022.08 - 2023.06)
- **유형**: 웹 플랫폼
- **설명**: POS 재고 관리 및 디지털 마케팅 솔루션 통합 기업 플랫폼
- **기술**: Django, Python, HTML/CSS, JS, MySQL, Docker
- **역할**: 프로젝트 매니저
- **팀**: 3명 (PM, 백엔드, UI/UX)
- **링크**: [fidesbankcard.com](https://fidesbankcard.com)

### 5. **Mocean** (2021.03 - 2021.12)
- **유형**: 웹 플랫폼
- **설명**: 의사 관리 패널과 예약 시스템을 갖춘 헬스케어 플랫폼
- **기술**: React, Python, Django, nginx, Docker, RESTful API
- **역할**: 프로젝트 리드
- **팀**: 3명
- **링크**: [moceanpt.com](https://moceanpt.com/)

### 6. **FD Holdings** (2021.03 - 2022.05)
- **유형**: 웹 플랫폼
- **설명**: 6개 사업부를 통합하는 기업 홀딩스 웹사이트
- **기술**: React, Next.js, Django, Python, Keras
- **역할**: 리드 개발자
- **팀**: 3명
- **링크**: [fdgroup.co.kr](https://fdgroup.co.kr/)

### 7. **Featuring Co** (2020.05 - 2020.09)
- **유형**: 웹 플랫폼
- **설명**: SEO 최적화 블로깅 플랫폼
- **기술**: Python, PostgreSQL, Google Analytics, TailwindCSS
- **역할**: 프론트엔드 개발자 & SEO 전문가
- **링크**: [featuring.co](https://featuring.co)

### 8. **ChartGet** (2023.01 - 2024.03)
- **유형**: 모바일 앱
- **설명**: 차트 분석 학습 및 마스터를 위한 크로스 플랫폼 앱
- **기술**: Flutter, Firebase, Dart, Hive/SQLite
- **역할**: 프로젝트 매니저
- **팀**: 3명
- **링크**: [chartgetalgo.com](https://chartgetalgo.com/)

### 9. **Woulduin Coin** (2021.01 - 2021.12) [판매됨]
- **유형**: 웹 & 모바일 앱
- **설명**: 한국 암호화폐 정보 플랫폼
- **기술**: React Native, MongoDB, Firebase, Redux, RESTful API
- **역할**: 프로젝트 매니저
- **팀**: 3명

### 10. **Metro Health Insurance** (2023.06 - 2024.02)
- **유형**: 웹 플랫폼
- **설명**: 보험 회사 통합 관리 시스템 및 디지털 마케팅 도구
- **기술**: HTML/CSS, Javascript, Django, Python, Google Analytics
- **역할**: 리스크 매니징, 디지털 마케팅, 개발 협업
- **링크**: [metrohealthins.com](https://www.metrohealthins.com/contact-us/)

---

## 🌍 다국어 지원

이 프로젝트는 **i18next**를 사용하여 완벽한 다국어 지원을 제공합니다.

### **지원 언어**
- 🇰🇷 한국어 (Korean)
- 🇺🇸 영어 (English)

### **언어 추가 방법**

1. `src/i18n/locales/` 디렉토리에 새로운 언어 파일 생성 (예: `ja.json`)
2. `src/i18n/index.ts`에서 새 언어 리소스 등록
3. 모든 프로젝트 데이터(`src/data/projects.ts`)에 새 언어 필드 추가

### **언어 전환**

헤더 우측 상단의 **EN/KR** 버튼을 클릭하면 즉시 언어가 전환됩니다.

---

## 🌓 테마 시스템

### **지원 테마**
- ☀️ 라이트 모드
- 🌙 다크 모드

### **테마 전환**

헤더의 태양/달 아이콘을 클릭하여 테마를 전환할 수 있습니다.

### **커스텀 훅: `useTheme`**

```typescript
const { theme, toggleTheme } = useTheme();
```

테마 설정은 `localStorage`에 저장되어 다음 방문 시에도 유지됩니다.

---

## 📱 반응형 디자인

### **브레이크포인트**

Tailwind CSS의 기본 브레이크포인트를 사용합니다:

- `sm`: 640px
- `md`: 768px
- `lg`: 1024px
- `xl`: 1280px
- `2xl`: 1536px

### **모바일 최적화**

- 터치 친화적인 UI
- 최적화된 이미지 로딩
- 부드러운 스크롤 애니메이션

---

## 🚢 배포

### **Netlify 배포**

이 프로젝트는 **Netlify**를 통해 배포됩니다.

#### **자동 배포 설정**

`netlify.toml` 파일에 배포 설정이 정의되어 있습니다:

```toml
[build]
  command = "npm run build"
  publish = "dist"
```

#### **배포 단계**

1. GitHub 리포지토리와 Netlify 연결
2. 빌드 명령어: `npm run build`
3. 배포 디렉토리: `dist`
4. 자동 배포 활성화

---

## 📊 성과 메트릭

각 프로젝트는 다음과 같은 성과 지표를 포함합니다:

- **marketReach**: 시장 도달률
- **conversion**: 전환율
- **retention**: 사용자 유지율
- **growth**: 성장률
- **satisfaction**: 만족도

---

## 🤝 기여

이 프로젝트는 개인 포트폴리오이지만, 피드백과 제안은 언제나 환영합니다!

### **피드백 제공 방법**

- 이슈 생성: [GitHub Issues](https://github.com/PyungkangHong094/PK_portfolio/issues)
- 이메일: your-email@example.com

---

## 📄 라이선스

이 프로젝트는 개인 포트폴리오로 제작되었습니다.

Copyright © 2024 Pyungkang Hong. All rights reserved.

---

## 📞 연락처

**Pyungkang Hong** (홍평강)

- 🌐 Portfolio: [ThinkPM](https://yourwebsite.com)
- 💼 LinkedIn: [Your LinkedIn](#)
- 📧 Email: your-email@example.com
- 🐙 GitHub: [@PyungkangHong094](https://github.com/PyungkangHong094)

---

<div align="center">
  
  **Made with ❤️ by Pyungkang Hong**
  
  ⭐ 이 프로젝트가 마음에 드셨다면 Star를 눌러주세요!
  
</div>