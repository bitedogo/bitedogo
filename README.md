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
* **Tech Stack:** `Next.js (App Router)` `TypeScript` `Supabase` `PostgreSQL` `TypeORM` `Vercel`
* **Links:** [🌐 공식 웹사이트](https://www.comeonoru.com) &nbsp;·&nbsp; [📦 GitHub Repo](https://github.com/bitedogo/ourmusicreview)

<br>

* **외부 음원 API 병렬 처리 및 캐싱 최적화**
  * <img src="https://img.shields.io/badge/Problem-red?style=flat-square"/> 다중 플랫폼(Spotify, iTunes, Deezer) 직렬 호출로 인한 **응답 지연 병목 발생**
  * <img src="https://img.shields.io/badge/Solution-blue?style=flat-square"/> `Promise.all` 기반 **서버사이드 병렬 호출** 및 **정규화 캐싱 파이프라인** 구축
  * <img src="https://img.shields.io/badge/Result-green?style=flat-square"/> 네트워크 Latency를 낮추고 **음원 스트리밍 링크 렌더링 체감 속도 대폭 개선**

* **세션 기반 중복 카운트 차단 및 DB 쓰기 부하 완화**
  * <img src="https://img.shields.io/badge/Problem-red?style=flat-square"/> 새로고침 및 본인 글 열람 시 **불필요한 `UPDATE` 쿼리 빈번 발생**
  * <img src="https://img.shields.io/badge/Solution-blue?style=flat-square"/> **세션 키 검증 인터셉트** 및 **작성자 본인 조회 필터링** 로직 적용
  * <img src="https://img.shields.io/badge/Result-green?style=flat-square"/> 무분별한 어뷰징 트래픽 억제 및 **불필요한 DB 트랜잭션 절감**

* **풀스택 아키텍처 구축 및 프로덕션 무중단 운영**
  * <img src="https://img.shields.io/badge/Focus-orange?style=flat-square"/> **Next.js App Router** 기반 **Server Component 분리**, **Dynamic OG / Sitemap 파이프라인** 세팅으로 검색 엔진 최적화(SEO) 환경 마련
  * <img src="https://img.shields.io/badge/Focus-orange?style=flat-square"/> **Supabase(PostgreSQL)** 모델링 및 **TypeORM** 기반 CRUD API 구축부터 **Vercel 실서버 배포·커스텀 도메인 운영**까지 전 과정 완수

---

### 🐱 자바냥 (JavaNyang) — 실시간 자바 퀴즈 배틀 플랫폼
> **"게이미피케이션 요소와 1:1 라이브 대전을 결합한 자바 학습 웹 서비스"**

* **Period:** 2025.05 ~ 2025.07 <img src="https://img.shields.io/badge/Released-blue?style=flat-square"/>
* **Team:** 6인 팀 (`Role: Team Leader / PM`, `DB 설계 40%`, `개발 20%`)
* **Tech Stack:** `React` `Next.js` `Supabase Realtime` `PostgreSQL` `Vite`
* **Links:** [🌐 서비스 데모](https://hyunsuplee.github.io/JavaNyang/) &nbsp;·&nbsp; [📦 GitHub Repo](https://github.com/hyunsupLee/JavaNyang)

<br>

* **Supabase Realtime 기반 대전 상태 Pub/Sub 동기화**
  * <img src="https://img.shields.io/badge/Problem-red?style=flat-square"/> 다중 라운드 대전 중 **방 상태, 참가자 레디, 답안 제출 데이터 싱크 누락 위험**
  * <img src="https://img.shields.io/badge/Solution-blue?style=flat-square"/> `postgres_changes` 구독 채널을 **방 단위/라운드 단위로 관심사 분리(Pub/Sub)**
  * <img src="https://img.shields.io/badge/Result-green?style=flat-square"/> 5라운드 실시간 대전 진행 간 **답안 제출 및 점수 판정 데이터 유실 없이 안정적 동기화**

* **학습 지속성을 높이는 게이미피케이션 엔진 설계**
  * <img src="https://img.shields.io/badge/Focus-orange?style=flat-square"/> 퀴즈 채점 결과에 따른 **동적 EXP 산정** 및 **실시간 레벨업 시스템** 구현
  * <img src="https://img.shields.io/badge/Focus-orange?style=flat-square"/> 출석 및 누적 정답 수 조건을 체크하는 **업적(`achievements`) 테이블 연동** 및 **실시간 리더보드** 구축

* **스프린트 리딩 및 기한 내 100% 릴리즈 달성**
  * <img src="https://img.shields.io/badge/Focus-orange?style=flat-square"/> **프로젝트 총괄(PM)**로서 요구사항 정의, DB 설계 주도 및 컴포넌트 인터페이스 규격화
  * <img src="https://img.shields.io/badge/Result-green?style=flat-square"/> 기획 단계 스펙(퀴즈/대전/채팅/업적)을 **스프린트 일정 내 완성하여 GitHub Pages로 배포**

---

### 📚 StudyO (스터디오) — 올인원 스터디 협업 플랫폼
> **"스터디 모집부터 일정 관리, 자료 공유를 통합한 협업 워크스페이스"**

* **Period:** 2025.07 ~ 2025.08 (5주) <img src="https://img.shields.io/badge/Completed-lightgrey?style=flat-square"/>
* **Team:** 6인 팀 (`프론트엔드 개발 20%`, `DB 모델링 30%`)
* **Tech Stack:** `Java` `Spring Boot` `MyBatis` `OracleDB` `React` `AWS S3`
* **Links:** [📦 Frontend Repo](https://github.com/hyunsupLee/react-study-o) &nbsp;·&nbsp; [📦 Backend Repo](https://github.com/hyunsupLee/tjspring)

<br>

* **React Portal 기반 공통 모달 프리셋 시스템 구축**
  * <img src="https://img.shields.io/badge/Problem-red?style=flat-square"/> 화면마다 모달 코드가 산발적으로 중복 작성되며 **유지보수 비용 및 UI 불일치 증가**
  * <img src="https://img.shields.io/badge/Solution-blue?style=flat-square"/> Confirm/Alert/Action 타입별 프리셋을 정의한 **전역 Portal 공통 모달 컴포넌트** 설계
  * <img src="https://img.shields.io/badge/Result-green?style=flat-square"/> 마이페이지·멤버 관리 등 전역의 **모달 작업 공수 단축** 및 **사용자 인터랙션 일관성 확보**

* **다중 스터디 일정 데이터 비동기 병렬화**
  * <img src="https://img.shields.io/badge/Problem-red?style=flat-square"/> 참여 스터디가 늘어남에 따라 **다중 일정 API 순차 호출로 인한 로딩 지연**
  * <img src="https://img.shields.io/badge/Solution-blue?style=flat-square"/> FullCalendar 연동 시 **다중 일정 비동기 병렬 호출** 및 **날짜별 단일 이벤트 매핑 구조 간소화**
  * <img src="https://img.shields.io/badge/Result-green?style=flat-square"/> 캘린더 렌더링 딜레이를 해소하고, `useMemo` 기반 **호스트 권한 분리로 비인가 조작 방어**

* **사전 검증 기반 클라이언트 파일 업로드 파이프라인**
  * <img src="https://img.shields.io/badge/Focus-orange?style=flat-square"/> 브라우저 단에서 **파일 확장자 및 용량 선검증** 후 `FormData` 전송하여 **잘못된 서버 요청 차단**
  * <img src="https://img.shields.io/badge/Focus-orange?style=flat-square"/> 업로드된 프로필 및 썸네일 이미지를 **AWS S3와 연동**해 안정적인 **정적 미디어 서빙 경로** 확립

---

<p align="center">
  © 2026 <b>bitedogo</b>. Built with passion & clean architecture.
</p>
