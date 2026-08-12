# 👋 Hi, I'm bitedogo!
### 🚀 Full Stack Developer Based in Seoul

> **"아이디어를 코드로 실현하고, 안정적이고 확장성 있는 시스템을 설계합니다."**  
> 대중적인 서비스를 위한 데이터 아키텍처 설계와 사용자 중심의 UX 개발에 몰입하는 풀스택 개발자입니다.

<p align="left">
  <a href="https://github.com/bitedogo"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
  <a href="mailto:your.email@example.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://instagram.com/your_id"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
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

### 💿 ORU (오루) — 음악 리뷰 및 소통 플랫폼
> **"국내 대중음악 리스너들을 위한 앨범 단위 평점 & 아카이빙 웹 서비스"**

* **Period:** 2025.10 ~ Present (Production)
* **Team:** 3인 팀 (`Role: 기획 100%`, `Dev 50%`, `DB 30%`)
* **Tech Stack:** `Next.js (App Router)` `TypeScript` `Supabase` `PostgreSQL` `TypeORM` `Vercel` `Cursor AI`
* **Links:** [🌐 Official Website](https://www.comeonoru.com) &nbsp;·&nbsp; [📦 GitHub Repo](https://github.com/bitedogo/ourmusicreview)

<br>

**1️⃣ 문제 정의 (Problem Statement)**
* **시장 부재:** 해외(RateYourMusic 등) 대비 국내에는 대중음악 리스너들이 앨범 단위로 심도 있게 리뷰를 나누고 아카이빙할 커뮤니티가 부재함.
* **기술적 병목 및 중복 카운트:** 다중 외부 음원 API 순차 호출로 인한 페이지 렌더링 지연, 그리고 무분별한 새로고침으로 조회수가 중복 집계되며 DB UPDATE가 불필요하게 늘어나는 이슈가 발생함.

**2️⃣ 가설 수립 및 성공 기준 (Hypothesis & Success Criteria)**
* **가설 1:** 외부 음원 API를 서버사이드 병렬 호출(`Promise.all`) 및 캐싱하면 탐색·링크 노출 속도가 개선될 것이다.
* **가설 2:** 세션 키 기반 중복 카운트 방지와 작성자 본인 제외 로직을 적용하면, 새로고침성 중복 조회와 불필요한 UPDATE를 줄일 수 있을 것이다.
* **성공/실패 판단 기준:**
  * 성공: 외부 음원 링크 로딩 체감 개선(병렬·캐싱) & 동일 세션 내 중복 조회·불필요 UPDATE 감소.
  * 실패: 외부 API 응답 실패율 증가, 또는 잘못된 플랫폼 링크 매칭 증가 시 Failure로 판단.

**3️⃣ 액션 및 검증 (Action & Validation)**
* **기획 & 아키텍처:** 100% 독자 기획. Next.js App Router 기반 SEO 기초(Sitemap·OG·서버 렌더링) 세팅 및 Supabase(PostgreSQL) + TypeORM 기반 CRUD/집계 API 구축.
* **AI 생산성 도입:** Cursor AI로 반복 CRUD 보일러플레이트 작성 시간을 단축하고, 도메인 로직·DB 설계에 집중.
* **성능 및 조회수 최적화:** iTunes/Odesli/Spotify/Deezer API 병렬 조회·정규화·캐싱 파이프라인 구축, 세션 키 기반 조회수 중복 방지 및 작성자 본인 제외 로직 구현.

**4️⃣ 결과 및 임팩트 (Result & Impact)**
* **실 상용화 달성:** 아이디어 빌딩부터 도메인 확보, Vercel 배포·운영까지 원스톱으로 완성.
* **중복 조회 억제 및 DB 부하 완화:** 동일 세션 중복 카운트와 작성자 자가 조회를 막아 불필요한 UPDATE를 줄임.
* **음악 탐색 인터페이스 응답 개선:** 외부 API 병렬화·캐싱으로 네트워크 latency를 줄이고 스트리밍 링크 노출을 안정화.

**5️⃣ 러닝 포인트 (Learning Points)**
* **SEO & SSR의 실질적 가치:** Client Component 위주에서 벗어나 Server Component와 Sitemap·OG 등 SEO 기초 세팅이 검색 노출 기반과 초기 로딩 경험에 미치는 영향을 체감.
* **AI 도구 활용 트레이드오프:** Cursor AI로 속도를 내는 동시에, 생성된 코드의 타입 안정성·아키텍처 적합성을 검증하는 안목의 중요성을 학습.

---

### 🐱 자바냥 (JavaNyang) — 온라인 자바 퀴즈 플랫폼
> **"Gamification 요소와 1:1 라이브 대전을 결합한 자바 학습 웹 플랫폼"**

* **Period:** 2025.05 ~ 2025.07
* **Team:** 6인 팀 (`Role: Team Leader / PM`, `DB 40%`, `Dev 20%`)
* **Tech Stack:** `React` `Next.js` `Supabase Realtime` `PostgreSQL` `Vite`
* **Links:** [🌐 Service Link](https://hyunsuplee.github.io/JavaNyang/) &nbsp;·&nbsp; [📦 GitHub Repo](https://github.com/hyunsupLee/JavaNyang)

<br>

**1️⃣ 문제 정의 (Problem Statement)**
* **학습 이탈율:** 단방향·혼자 풀이 중심의 프로그래밍 학습은 초급자의 지속 학습 동기가 약하고 이탈로 이어지기 쉬움.
* **실시간 대전 UX:** 1:1 퀴즈 대전에서 방 상태·참가자·라운드 답안이 어긋나면 공정한 대결 경험이 깨짐.

**2️⃣ 가설 수립 및 성공 기준 (Hypothesis & Success Criteria)**
* **가설 1:** 퀴즈 기반 게이미피케이션(EXP·레벨·업적·랭킹)과 1:1 라이브 대전을 도입하면 학습 지속 동기가 강화될 것이다.
* **가설 2:** Supabase Realtime으로 방·참가자·라운드 답안을 구독해 동기화하면, 방 로비 기반 1:1 대전도 안정적인 라이브 UX를 유지할 수 있을 것이다.
* **성공/실패 판단 기준:**
  * 성공: 방 생성·입장·준비·5라운드 진행까지 상태 동기화가 끊기지 않고, 기획한 핵심 기능(퀴즈·대전·업적·채팅)이 일정 내 릴리즈됨.
  * 실패: 대전 중 방/참가자/답안 동기화 실패로 라운드 진행이 불가하거나, 핵심 기능이 미완성인 채 마감되는 경우.

**3️⃣ 액션 및 검증 (Action & Validation)**
* **팀 리딩 & PM:** 프로젝트 총괄로서 요구사항 정리·스프린트 관리, Supabase(PostgreSQL) 테이블·관계 설계 주도.
* **게이미피케이션 설계:** 퀴즈 정답 시 reward 기반 EXP·레벨 산정, 출석·정답 수·레벨 조건의 업적(`achievements` / `user_achievements`) 트리거 및 랭킹 연동.
* **실시간 파이프라인 구현:** Supabase Realtime(`postgres_changes`)으로 배틀 방·참가자·라운드 답안 동기화, 방 목록 로비 기반 1:1 매칭, 전역 실시간 채팅 구현.

**4️⃣ 결과 및 임팩트 (Result & Impact)**
* **1:1 라이브 대전 UX 확보:** Realtime 구독으로 방 상태·준비·라운드·점수를 동기화해 공정한 퀴즈 대전 경험 제공.
* **게이미피케이션으로 학습 루프 완성:** EXP·레벨·업적·랭킹으로 단기 성취와 재도전 동기를 연결.
* **일정 내 안정 릴리즈:** 2025.05~07 기획·개발·발표 일정에 맞춰 GitHub Pages로 서비스 배포.

**5️⃣ 러닝 포인트 (Learning Points)**
* **실시간 이벤트 기반 아키텍처:** 테이블 변경을 무분별하게 구독하면 상태가 복잡·불안정해지므로, 방·참가자·답안 등 필요한 단위로 Pub/Sub을 나누는 설계가 중요함을 체득.
* **팀 리더십 및 커뮤니케이션:** 기획–개발 간 요구사항 간극을 조기에 맞추고 스프린트를 조율하는 PM 역할의 중요성을 정립.

---

### 📚 StudyO (스터디오) — 올인원 스터디 협업 플랫폼
> **"스터디 모집부터 일정, 자료 공유까지 한 곳에서 처리하는 통합 워크스페이스"**

* **Period:** 2025.07 ~ 2025.08 (5 Weeks)
* **Team:** 6인 팀 (`Role: Dev 20%`, `DB 30%`)
* **Tech Stack:** `Java` `Spring Boot` `MyBatis` `OracleDB` `React` `AWS S3`
* **Links:** [📦 GitHub Frontend](https://github.com/hyunsupLee/react-study-o) &nbsp;·&nbsp; [📦 GitHub Backend](https://github.com/hyunsupLee/tjspring)

<br>

**1️⃣ 문제 정의 (Problem Statement)**
* **모달 UI 중복:** 확인/알림 모달이 화면마다 비슷한 구조로 반복되어, 문구·버튼·성공/실패 UI를 매번 따로 맞추는 비용이 큼.
* **일정 조회 복잡도:** 마이페이지에서 참여 스터디가 늘수록 그룹별 캘린더 API를 여러 번 호출·병합해야 해, 로딩·표시 로직이 무거워짐.

**2️⃣ 가설 수립 및 성공 기준 (Hypothesis & Success Criteria)**
* **가설 1:** Confirm형 모달을 type 프리셋(수락/추방/탈퇴/프로필 수정 등)으로 공통화하면, 동일 UI를 화면마다 새로 짜는 비용을 줄일 수 있다.
* **가설 2:** 스터디별 일정 조회를 병렬 처리하고, FullCalendar 연동 시 이벤트 매핑을 단순화하면 누적 일정 화면의 체감 지연을 줄일 수 있다.
* **성공/실패 판단 기준:**
  * 성공: Confirm/알림 흐름을 공통 컴포넌트·헬퍼로 재사용해, 신규 화면에서도 동일 패턴으로 모달을 붙일 수 있을 것. 마이페이지·스터디 캘린더에서 일정이 누락·꼬임 없이 표시되고, 호스트 권한에 따른 등록/수정이 안정적으로 동작할 것.
  * 실패: 스터디 병렬 조회 시 데이터 파싱 싱크가 깨지거나 권한별 CRUD 제어 실패 시 판단.

**3️⃣ 액션 및 검증 (Action & Validation)**
* **공통 Confirm 모달:** `ConfirmModal`을 Portal 기반으로 두고, 작업 유형별 프리셋·성공 모드를 정의해 마이페이지·멤버 관리 등에서 재사용.
* **캘린더 연동 정리:** `FullCalendar`로 스터디 일정 CRUD를 구현하고, 마이페이지에서는 참여 스터디 일정을 병렬 조회 후 날짜별 표시. 호스트 여부는 `useMemo`로 판별해 등록 권한을 분리.
* **파일 업로드 검증:** 프로필/썸네일·첨부 업로드 시 용량·이미지 타입을 프론트에서 선검증하고, `FormData`로 API에 전달. 저장된 이미지는 AWS S3 경로로 서빙.

**4️⃣ 결과 및 임팩트 (Result & Impact)**
* **모달 작성 공수 감소:** 확인/성공 UI를 프리셋으로 통일해, 화면마다 모달 마크업·문구를 중복 작성하는 범위를 줄임.
* **일정 UX 안정화:** 스터디·마이페이지 캘린더에서 일정 조회·등록·수정 흐름을 일관되게 유지하고, 다중 스터디 일정도 한 화면에서 확인 가능.
* **업로드 안정성 향상:** 잘못된 파일 형식·과도한 용량을 업로드 전에 걸러, 서버 전송 실패·불필요 요청을 줄임.

**5️⃣ 러닝 포인트 (Learning Points)**
* **재사용 가능한 UI 계약 (UI Contract):** 동작만 맞추는 UI가 아니라, type/프리셋처럼 팀원이 바로 가져다 쓸 수 있는 공통 컴포넌트 경계를 정하는 것이 유지보수에 더 중요하다는 점.
* **데이터 흐름 중심 성능 감각:** 렌더 최적화 이전에 “API를 몇 번 치는지·파싱을 어디서 하는지”를 먼저 정리하는 것이 체감 성능에 직결된다는 점.

---

<p align="center">
  © 2026 <b>bitedogo</b>. Built with passion & clean architecture.
</p>
