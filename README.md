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

### 🛠️ Development & Productivity Tools
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

* **Period:** 2025.10 ~ Present (Production)
* **Team:** 3인 팀 (`기획 100%`, `풀스택 개발 50%`, `DB 설계 30%`)
* **Tech Stack:** `Next.js (App Router)` `TypeScript` `Supabase` `PostgreSQL` `TypeORM` `Vercel`
* **Links:** [🌐 Official Website](https://www.comeonoru.com) &nbsp;·&nbsp; [📦 GitHub Repo](https://github.com/bitedogo/ourmusicreview)

**Key Responsibilities & Engineering**
* **외부 음원 API 병렬 처리 및 캐싱**
  * 다중 스트리밍 플랫폼(Spotify, iTunes, Deezer 등) 링크 탐색 시 발생하는 직렬 호출 병목을 `Promise.all` 기반 병렬 호출 및 캐싱 파이프라인으로 개선하여 네트워크 latency 최소화
* **세션 기반 중복 집계 방지 및 쿼리 최적화**
  * 무분별한 새로고침으로 인한 불필요한 조회수 `UPDATE`를 방지하기 위해 세션 키 기반 검증 및 작성자 본인 조회 제외 로직 구현
* **풀스택 아키텍처 구축 및 실서버 운영**
  * Next.js App Router 기반 Server Component 분리와 Dynamic OG/Sitemap 적용으로 검색 엔진 최적화(SEO) 환경 마련
  * Supabase(PostgreSQL) 모델링 및 TypeORM 기반 CRUD API 구축, Vercel 실서버 배포 및 커스텀 도메인 운영 완수

---

### 🐱 자바냥 (JavaNyang) — 실시간 자바 퀴즈 배틀 플랫폼
> **"게이미피케이션과 1:1 라이브 대전을 결합한 자바 학습 웹 서비스"**

* **Period:** 2025.05 ~ 2025.07
* **Team:** 6인 팀 (`Role: Team Leader / PM`, `DB 설계 40%`, `Dev 20%`)
* **Tech Stack:** `React` `Next.js` `Supabase Realtime` `PostgreSQL` `Vite`
* **Links:** [🌐 Service Demo](https://hyunsuplee.github.io/JavaNyang/) &nbsp;·&nbsp; [📦 GitHub Repo](https://github.com/hyunsupLee/JavaNyang)

**Key Responsibilities & Engineering**
* **Supabase Realtime 기반 1:1 대전 상태 동기화**
  * `postgres_changes` 구독 채널을 방 상태·라운드 답안·채팅 등 목적별로 분리하여 다중 라운드 실시간 대전 진행 중 상태 유실 없는 안정적인 Pub/Sub 환경 구현
* **학습 지속을 위한 게이미피케이션 엔진 설계**
  * 퀴즈 정답 결과에 따른 동적 EXP 산정 및 레벨업 시스템 구현
  * 출석 일수 및 누적 정답 수 조건을 추적하는 업적(`achievements`) 테이블 연동 및 실시간 랭킹 시스템 설계
* **스프린트 리딩 및 기한 내 릴리즈**
  * 요구사항 명세화 및 컴포넌트별 인터페이스 정의를 주도하여 대전·퀴즈·채팅 등 핵심 기능을 기획 일정 내 안정적으로 배포

---

### 📚 StudyO (스터디오) — 올인원 스터디 협업 플랫폼
> **"스터디 모집부터 일정 관리, 자료 공유를 통합한 협업 워크스페이스"**

* **Period:** 2025.07 ~ 2025.08 (5 Weeks)
* **Team:** 6인 팀 (`Dev 20%`, `DB 모델링 30%`)
* **Tech Stack:** `Java` `Spring Boot` `MyBatis` `OracleDB` `React` `AWS S3`
* **Links:** [📦 Frontend Repo](https://github.com/hyunsupLee/react-study-o) &nbsp;·&nbsp; [📦 Backend Repo](https://github.com/hyunsupLee/tjspring)

**Key Responsibilities & Engineering**
* **React Portal 기반 공통 모달 프리셋 시스템 구축**
  * 확인/알림 모달 UI를 유형별 프리셋(Confirm/Alert/Action)으로 추상화하여 마이페이지·멤버 관리 등 전역에서 재사용 가능한 인터페이스 확립 및 중복 코드 제거
* **다중 스터디 일정 조회 및 캘린더 동기화**
  * FullCalendar 연동 시 참여 중인 여러 스터디의 일정 데이터를 비동기 병렬 처리하고 이벤트 매핑 로직을 최적화하여 렌더링 안정성 확보
  * `useMemo` 기반의 호스트 권한 판별 로직 분리로 비인가 사용자의 일정 수정/등록 차단
* **클라이언트 사전 검증 기반 파일 업로드 파이프라인**
  * 파일 확장자 및 용량을 브라우저 단에서 1차 선검증 후 `FormData`로 전달해 불필요한 서버 부하 방지
  * 프로필 및 썸네일 이미지를 AWS S3와 연동하여 정적 파일 서빙 경로 구축

---

<p align="center">
  © 2026 <b>bitedogo</b>. Built with passion & clean architecture.
</p>
