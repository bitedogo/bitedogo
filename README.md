# 👋 Hi, I'm bitedogo
### Full Stack Developer Based in Seoul

> **아이디어를 코드를 통해 현실로 만들어내는 과정에 몰입합니다.**
> <mark><b>확장성 있는 웹 애플리케이션</b></mark>과 <mark><b>안정적인 데이터 아키텍처</b></mark>를 설계하는 풀스택 개발자입니다.

[GitHub](https://github.com/bitedogo) &nbsp;·&nbsp; [Email](mailto:your.email@example.com) &nbsp;·&nbsp; [Instagram](https://instagram.com/your_id)

---

## 🚀 About Me

* **📍 Location:** 대한민국 서울
* **💻 Languages:** JavaScript, TypeScript, Java, Dart
* **🎯 Focus:** RESTful/Hybrid API 설계, 데이터베이스 최적화, 실시간 동기화 서비스 구현

---

## 🛠️ Technology Stack

### Languages & Frontend
<img src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=flat-square&logo=java&logoColor=white" alt="Java"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/dart-%230175C2.svg?style=flat-square&logo=dart&logoColor=white" alt="Dart"/> &nbsp;&nbsp;·&nbsp;&nbsp; <img src="https://img.shields.io/badge/Next.js-black?style=flat-square&logo=next.js&logoColor=white" alt="Next.js"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/react-%2320232a.svg?style=flat-square&logo=react&logoColor=%2361DAFB" alt="React"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/vue.js-%234FC08D.svg?style=flat-square&logo=vue.js&logoColor=white" alt="Vue.js"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=flat-square&logo=tailwind-css&logoColor=white" alt="Tailwind CSS"/>

### Backend & Database
<img src="https://img.shields.io/badge/spring_boot-%236DB33F.svg?style=flat-square&logo=spring-boot&logoColor=white" alt="Spring Boot"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/node.js-6DA55F?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/> &nbsp;&nbsp;·&nbsp;&nbsp; <img src="https://img.shields.io/badge/supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" alt="Supabase"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/postgresql-%23316192.svg?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=oracle&logoColor=white" alt="Oracle"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/AWS_S3-569A31?style=flat-square&logo=amazons3&logoColor=white" alt="AWS S3"/>

### Tools
<img src="https://img.shields.io/badge/git-%23F05033.svg?style=flat-square&logo=git&logoColor=white" alt="Git"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/github-%23181717.svg?style=flat-square&logo=github&logoColor=white" alt="GitHub"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/vercel-%23000000.svg?style=flat-square&logo=vercel&logoColor=white" alt="Vercel"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/figma-%23F24E1E.svg?style=flat-square&logo=figma&logoColor=white" alt="Figma"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/intellij_idea-%23000000.svg?style=flat-square&logo=intellij-idea&logoColor=white" alt="IntelliJ IDEA"/>&nbsp;&nbsp; <img src="https://img.shields.io/badge/Visual_Studio_Code-007ACC?style=flat-square&logo=visual-studio-code&logoColor=white" alt="VS Code"/>

---

## 🎯 Featured Projects

### 💿 ORU (오루) — 음악 리뷰 및 소통 플랫폼
> 앨범 단위 평점 기록 및 음악 리스너 간의 취향 교감을 제공하는 풀스택 웹 서비스

* **기간:** 2025.10 ~ 현재 (진행 중)
* **기여:** 3인 팀 (본인 기여도: 기획 및 아이디어 발제 100%, 개발 50%, DB 설계 30%)
* **기술:** `Next.js` &nbsp;&nbsp; `TypeScript` &nbsp;&nbsp; `Supabase (PostgreSQL)` &nbsp;&nbsp; `TypeORM` &nbsp;&nbsp; `Vercel` &nbsp;&nbsp; `Cursor AI`
* **링크:** [Official Website](https://www.comeonoru.com) &nbsp;·&nbsp; [GitHub Repository](https://github.com/bitedogo/ourmusicreview)

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
> 기초 문법부터 고급 개념까지 한 손으로 즐기는 웹/모바일 반응형 자바 프로필 학습 플랫폼

* **기간:** 2025.05 ~ 2025.07
* **기여:** 6인 팀 (Team Leader / 본인 기여도: DB 설계 40%, 개발 20%)
* **기술:** `React` &nbsp;&nbsp; `Next.js` &nbsp;&nbsp; `Supabase Realtime` &nbsp;&nbsp; `PostgreSQL` &nbsp;&nbsp; `Vite`
* **링크:** [Service Link](https://hyunsuplee.github.io/JavaNyang/) &nbsp;·&nbsp; [GitHub Repository](https://github.com/hyunsupLee/JavaNyang)

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
> 스터디 모집, 팀 빌딩, 체계적인 일정 관리 및 파일 공유를 지원하는 통합 관리 솔루션

* **기간:** 2025.07 ~ 2025.08 (5주)
* **기여:** 6인 팀 (본인 기여도: DB 설계 30%, 개발 20%)
* **기술:** `Java` &nbsp;&nbsp; `Spring Boot` &nbsp;&nbsp; `MyBatis` &nbsp;&nbsp; `OracleDB` &nbsp;&nbsp; `React` &nbsp;&nbsp; `AWS S3`
* **링크:** [GitHub Frontend](https://github.com/hyunsupLee/react-study-o) &nbsp;·&nbsp; [GitHub Backend](https://github.com/hyunsupLee/tjspring)

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
© 2026 bitedogo. All rights reserved.
