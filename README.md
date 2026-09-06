# 👋 Hi, I'm bitedogo!
### 🚀 Full Stack Developer Based in Seoul

> **"아이디어를 코드로 실현하고, 안정적이고 확장성 있는 시스템을 설계합니다."**  
> 대중적인 서비스를 위한 데이터 아키텍처 설계와 사용자 중심의 UX 개발에 몰입하는 풀스택 개발자입니다.

<p align="left">
  <a href="https://github.com/bitedogo"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
  <a href="mailto:forsix5020@naver.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://instagram.com/rexisfine"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
</p>

---

## 🛠️ Tech Stack & Tools

### 🌐 Frontend & Languages
<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=TypeScript&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=JavaScript&logoColor=black"/>
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=Next.js&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=black"/>
  <img src="https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=TailwindCSS&logoColor=white"/>
  <img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=Dart&logoColor=white"/>
</p>

### ⚙️ Backend & Database
<p>
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=Java&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=SpringBoot&logoColor=white"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=Node.js&logoColor=white"/>
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=Supabase&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=PostgreSQL&logoColor=white"/>
  <img src="https://img.shields.io/badge/OracleDB-F80000?style=flat-square&logo=Oracle&logoColor=white"/>
  <img src="https://img.shields.io/badge/TypeORM-FE0803?style=flat-square&logo=TypeORM&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS_S3-569A31?style=flat-square&logo=AmazonS3&logoColor=white"/>
</p>

### 🛠️ Development & AI Productivity Tools
<p>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=Git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=GitHub&logoColor=white"/>
  <img src="https://img.shields.io/badge/Cursor_AI-000000?style=flat-square&logo=cursor&logoColor=white"/>
  <img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=Vercel&logoColor=white"/>
  <img src="https://img.shields.io/badge/IntelliJ_IDEA-000000?style=flat-square&logo=IntelliJIDEA&logoColor=white"/>
  <img src="https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=VisualStudioCode&logoColor=white"/>
</p>

---

## 🎯 Featured Projects

### 💿 ORU (오루) — 음악 리뷰 및 아카이빙 플랫폼
> **"국내 대중음악 리스너를 위한 앨범 단위 평점 & 아카이빙 웹 서비스"**

* **Period:** 2025.10 ~ 현재 <img src="https://img.shields.io/badge/Production-brightgreen?style=flat-square"/>
* **Team:** 3인 팀 (`기획 100%`, `풀스택 개발 50%`, `DB 설계 30%`)
* **Tech Stack:** `Next.js (App Router)` `TypeScript` `Supabase (PostgreSQL)` `TypeORM` `Vercel`
* **Links:** [🌐 공식 웹사이트](https://www.comeonoru.com) &nbsp;·&nbsp; [📦 GitHub Repo](https://github.com/bitedogo/ourmusicreview)

<br>

* **서버리스 환경 DB 연결 안정화 및 트랜잭션 최적화**
  * 서버리스 인스턴스 기동 시 발생하는 커넥션 고갈을 방지하기 위해 **인스턴스당 연결 풀 제한** 및 **DB 재연결 래퍼 로직** 구축
  * 다중 쓰기 작업에 **TypeORM 원자적 트랜잭션**을 적용하여 간헐적 500 에러 해결 및 데이터 정합성 보장

* **데이터베이스 모델링 및 조회 성능 튜닝**
  * 유저/앨범/리뷰 핵심 도메인 **외래키(FK) 정규화** 및 댓글·좋아요 대상 **다형 외래키 구조** 설계
  * 빈번한 목록 조회를 지원하기 위해 앨범 ID, 유저 ID, 알림 생성일자에 **수동 복합 인덱스(B-Tree)** 구축
  * 다중 조인 및 집계(`COUNT`, `GROUP BY`) 쿼리 튜닝으로 대용량 목록 서빙 지연 최소화

* **외부 API 병렬화 및 보안 인증 파이프라인 구축**
  * 다중 음원 플랫폼(Spotify, iTunes 등) 순차 조회 병목을 `Promise.all` **병렬 처리 및 캐싱**으로 개선
  * **Resend API**를 도입해 유효시간(TTL) 기반 임시 토큰 생성 및 **비밀번호 재설정 인증 파이프라인** 구현
  * **Next.js App Router** 기반 SSR 및 Dynamic OG/Sitemap 구축으로 검색 엔진 최적화(SEO) 환경 완성

---

### 🐱 자바냥 (JavaNyang) — 실시간 자바 퀴즈 배틀 플랫폼
> **"게이미피케이션 요소와 1:1 라이브 대전을 결합한 자바 학습 웹 서비스"**

* **Period:** 2025.05 ~ 2025.07 <img src="https://img.shields.io/badge/Released-blue?style=flat-square"/>
* **Team:** 6인 팀 (`Role: Team Leader / PM`, `DB 설계 40%`, `개발 20%`)
* **Tech Stack:** `React` `Next.js` `Supabase Realtime` `PostgreSQL` `Vite`
* **Links:** [🌐 서비스 데모](https://hyunsuplee.github.io/JavaNyang/) &nbsp;·&nbsp; [📦 GitHub Repo](https://github.com/hyunsupLee/JavaNyang)

<br>

* **Supabase Realtime 기반 대전 상태 Pub/Sub 동기화**
  * `postgres_changes` 구독 채널을 방 상태·라운드 답안·채팅 등 **목적별 채널로 분리(Pub/Sub)**
  * 5라운드 실시간 대전 진행 간 답안 제출 및 점수 판정 데이터 유실 없이 안정적인 상태 동기화 구현

* **학습 지속성을 높이는 게이미피케이션 엔진 설계**
  * 퀴즈 채점 결과에 따른 **동적 EXP 산정** 및 **실시간 레벨업 시스템** 구현
  * 출석 및 누적 정답 수 조건을 추적하는 **업적(`achievements`) 테이블 연동** 및 **실시간 리더보드** 구축

* **스프린트 리딩 및 기한 내 100% 릴리즈 달성**
  * **프로젝트 총괄(PM)**로서 요구사항 정의, 데이터 모델링 주도 및 컴포넌트 인터페이스 규격화
  * 기획 단계 핵심 스펙(퀴즈/대전/채팅/업적)을 일정 내 완성하여 GitHub Pages로 배포 완료

---

### 📚 StudyO (스터디오) — 올인원 스터디 협업 플랫폼
> **"스터디 모집부터 일정 관리, 자료 공유를 통합한 협업 워크스페이스"**

* **Period:** 2025.07 ~ 2025.08 (5주) <img src="https://img.shields.io/badge/Completed-lightgrey?style=flat-square"/>
* **Team:** 6인 팀 (`프론트엔드 개발 20%`, `DB 모델링 30%`)
* **Tech Stack:** `Java` `Spring Boot` `MyBatis` `OracleDB` `React` `AWS S3`
* **Links:** [📦 Frontend Repo](https://github.com/hyunsupLee/react-study-o) &nbsp;·&nbsp; [📦 Backend Repo](https://github.com/hyunsupLee/tjspring)

<br>

* **이벤트 기반 비동기 상태 동기화 및 메모리 누수 방지**
  * 마이페이지 프로필 수정 시 컴포넌트 간 로컬 State 불일치 문제를 해결하기 위해 브라우저 표준 **`CustomEvent` 발행-구독** 구조 도입
  * 컴포넌트 언마운트 시점에 **`removeEventListener` 클린업 함수**를 철저히 작성해 메모리 누수 원천 차단

* **다중 스터디 일정 조회 최적화 및 권한 제어**
  * FullCalendar 연동 시 다중 스터디 일정 API를 `Promise.all` 기반 **비동기 병렬 호출**로 처리해 렌더링 지연 해소
  * `useMemo` 기반의 호스트 권한 판별 로직을 분리해 비인가 사용자의 일정 조작 방지

* **선검증 기반 미디어 업로드 및 인프라 연동**
  * 브라우저 단에서 **파일 확장자 및 용량 선검증** 후 `FormData`로 전달해 불필요한 서버 요청 차단
  * **AWS S3** 버킷과 연동하여 스터디 프로필/썸네일 이미지의 안정적인 정적 미디어 서빙 경로 구축

---

<p align="center">
  © 2026 <b>bitedogo</b>. Built with passion & clean architecture.
</p>
