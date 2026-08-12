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

## 📊 GitHub Analytics

<p align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=bitedogo&show_icons=true&theme=radical&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=bitedogo&layout=compact&theme=radical&hide=c,html,css"/>
</p>
<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=bitedogo&theme=radical"/>
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
* **국내 음악 리뷰 커뮤니티 부재:** 해외(RateYourMusic 등) 대비 앨범 단위 전문 리뷰·아카이빙 플랫폼 미비.
* **API 병목 & 조회수 중복 UPDATE:** 다중 음원 API 순차 호출에 따른 Latency 및 무분별한 새로고침으로 인한 DB 부하.

**2️⃣ 가설 수립 및 성공 기준 (Hypothesis & Success Criteria)**
* **가설 1:** 외부 API 서버사이드 병렬 호출(`Promise.all`) 및 캐싱 적용 시 링크 노출 지연 개선.
* **가설 2:** 세션 키 기반 중복 카운트 방지 및 자가 조회 제외 적용 시 불필요한 DB `UPDATE` 쿼리 절감.
* **성공 기준:** 외부 음원 링크 로딩 체감 개선 및 동일 세션 내 중복 카운트 차단 / **실패 기준:** API 응답 실패율 증가 또는 링크 오매칭 발생.

**3️⃣ 액션 및 검증 (Action & Validation)**
* **기획 & 아키텍처:** 100% 독자 기획 및 Next.js App Router 기반 SEO(Sitemap·OG) 인프라 세팅.
* **AI 개발 생산성 극대화:** Cursor AI를 활용해 반복적인 CRUD 보일러플레이트 작성 단축 후 핵심 도메인 로직에 집중.
* **파이프라인 최적화:** iTunes/Odesli/Spotify/Deezer API 병렬 파이프라인 구축 및 세션 키 기반 조회수 검증 구현.

**4️⃣ 결과 및 임팩트 (Result & Impact)**
* **실 서비스 상용화 완료:** 기획부터 도메인 연결, Vercel 상용 배포까지 전 과정 원스톱 구축.
* **DB 부하 제어:** 동일 세션 중복 집계 차단으로 불필요한 WRITE 트래픽 절감.
* **UI 반응성 향상:** 외부 음원 데이터 가공 및 병렬 처리로 링크 노출 UX 안정화.

**5️⃣ 러닝 포인트 (Learning Points)**
* **SEO & SSR:** Server Component 구조와 메타데이터 설계가 검색 노출 및 초기 UX에 미치는 실질적 영향을 경험.
* **AI 도구 핸들링:** AI 생성 코드의 타입 안정성과 엔티티 적합성을 직접 검증·정제하는 코드 리뷰 안목 형성.

---

### 🐱 자바냥 (JavaNyang) — 온라인 자바 퀴즈 플랫폼
> **"Gamification 요소와 1:1 라이브 대전을 결합한 자바 학습 웹 플랫폼"**

* **Period:** 2025.05 ~ 2025.07
* **Team:** 6인 팀 (`Role: Team Leader / PM`, `DB 40%`, `Dev 20%`)
* **Tech Stack:** `React` `Next.js` `Supabase Realtime` `PostgreSQL` `Vite`
* **Links:** [🌐 Service Link](https://hyunsuplee.github.io/JavaNyang/) &nbsp;·&nbsp; [📦 GitHub Repo](https://github.com/hyunsupLee/JavaNyang)

<br>

**1️⃣ 문제 정의 (Problem Statement)**
* **학습 이탈률:** 초급자의 단방향 프로그래밍 학습 이탈 방지를 위한 실시간 동기부여 요소 필요.
* **실시간 상태 동기화:** 1:1 퀴즈 대전 시 방 상태·참가자·답안 데이터의 레이스 조건(Race Condition) 해결 필요.

**2️⃣ 가설 수립 및 성공 기준 (Hypothesis & Success Criteria)**
* **가설 1:** 퀴즈 게이미피케이션(EXP/레벨/업적/랭킹) 도입 시 지속 학습 루프 형성 가능.
* **가설 2:** Supabase Realtime 기반 이벤트 구독 적용 시 1:1 대전 상태 라이브 동기화 가능.
* **성공 기준:** 5라운드 매칭 진행 동안 동기화 단락 없이 정시 릴리즈 / **실패 기준:** 대전 중 싱크 어긋남으로 게임 진행 불가.

**3️⃣ 액션 및 검증 (Action & Validation)**
* **PM & DB 설계:** 6인 스프린트 일정 관리 및 PostgreSQL 릴레이션 스키마 주도 설계.
* **게이미피케이션 로직:** 정답 Reward 가중치 계산, 출석/정답 수 트리거 기반 `achievements` 테이블 연동.
* **실시간 파이프라인:** Supabase Realtime(`postgres_changes`)을 통한 1:1 배틀 룸, 로비 대기열 및 전역 채팅 구축.

**4️⃣ 결과 및 임팩트 (Result & Impact)**
* **안정적인 1:1 대전 UX:** Realtime 이벤트 파이프라인 기반으로 라이브 점수 및 진행 상태 동기화.
* **학습 지속 루프 형성:** 경험치/레벨/업적 시스템 연동으로 유저 참여 자극.
* **정시 배포 완료:** GitHub Pages 기반 배포 마일스톤 준수.

**5️⃣ 러닝 포인트 (Learning Points)**
* **Pub/Sub 아키텍처:** 무분별한 구독 사용의 비효율성을 체감하고 도메인 단위로 이벤트를 분리하는 실시간 설계 감각 습득.
* **프로젝트 리더십:** 기획과 개발 간 병목 요인을 사전에 제거하는 아키텍트/PM 역할 정립.

---

### 📚 StudyO (스터디오) — 올인원 스터디 협업 플랫폼
> **"스터디 모집부터 일정, 자료 공유까지 한 곳에서 처리하는 통합 워크스페이스"**

* **Period:** 2025.07 ~ 2025.08 (5 Weeks)
* **Team:** 6인 팀 (`Role: Dev 20%`, `DB 30%`)
* **Tech Stack:** `Java` `Spring Boot` `MyBatis` `OracleDB` `React` `AWS S3`
* **Links:** [📦 GitHub Frontend](https://github.com/hyunsupLee/react-study-o) &nbsp;·&nbsp; [📦 GitHub Backend](https://github.com/hyunsupLee/tjspring)

<br>

**1️⃣ 문제 정의 (Problem Statement)**
* **컴포넌트 코드 중복:** 다수 화면에서 유사한 Modal UI가 반복 구현되어 코드 파편화 심화.
* **일정 데이터 로딩 복잡도:** 다중 스터디 참여 유저의 마이페이지 캘린더 파싱 로직 및 호출 비효율.

**2️⃣ 가설 수립 및 성공 기준 (Hypothesis & Success Criteria)**
* **가설 1:** Confirm형 모달을 Type 프리셋 구조로 표준화 시 UI 작성 중복 코드 단축 가능.
* **가설 2:** 스터디별 일정 API 병렬 처리 및 이벤트 매핑 단순화 시 캘린더 렌더링 지연 감소.
* **성공 기준:** 공통 모달 패턴 재사용성 확보 및 권한별 CRUD 정상 동작 / **실패 기준:** 병렬 조회 데이터 파싱 오차 발생.

**3️⃣ 액션 및 검증 (Action & Validation)**
* **공통 UI 모달 패턴:** Portal 기반 `ConfirmModal` 및 작업 유형별 프리셋 설계로 모달 재사용성 극대화.
* **캘린더 & 권한 제어:** FullCalendar 연동, 참여 스터디 일정 병렬 파싱 및 `useMemo` 기반 호스트 CRUD 권한 분리.
* **S3 업로드 검증:** 이미지 타입/용량 클라이언트 선검증 적용 및 `FormData` 기반 AWS S3 연동.

**4️⃣ 결과 및 임팩트 (Result & Impact)**
* **개발 공수 단축:** 프리셋 기반 공통 모달 도입으로 마크업 중복 작성 대폭 감소.
* **일정 UX 안정화:** 다중 스터디 일정 데이터를 일관된 흐름으로 정돈하여 한 화면에서 제공.
* **클라이언트 단 사전 검증:** 부적절한 파일 업로드 차단을 통해 백엔드 예외 발생율 감소.

**5️⃣ 러닝 포인트 (Learning Points)**
* **UI Contract 정립:** 단순히 렌더링만 처리하는 컴포넌트가 아닌, 팀 생산성을 높이는 공통 컴포넌트 인터페이스 설계의 중요성 경험.
* **데이터 흐름 최적화:** 브라우저 렌더링 이전에 데이터 파싱 및 API 요청 횟수를 줄이는 것이 UX 성능에 직결됨을 확인.

---

<p align="center">
  © 2026 <b>bitedogo</b>. Built with passion & clean architecture.
</p>
