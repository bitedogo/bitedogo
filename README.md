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
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=white"/>
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

* **서버리스 환경 DB 연결 안정화 및 트랜잭션 관리**
  * Vercel 서버리스 환경의 인스턴스별 풀 확장을 고려해 프로덕션 **TypeORM 커넥션 풀을 인스턴스당 1개로 제한**하고 **유휴·연결 타임아웃** 설정
  * 끊긴 풀에서 쿼리 실패 시 1회 재연결 후 재시도하는 **`withDatabase` 래퍼**를 설계해 리뷰 API 및 세션 조회에 적용
  * 릴리즈 노트 미러링 등 다중 쓰기가 한 단위인 작업에 **TypeORM 트랜잭션**을 적용하여 데이터 부분 저장 방지

* **데이터베이스 모델링 및 조회 성능 최적화**
  * 유저·앨범·리뷰 도메인을 FK로 정규화하고, 댓글·좋아요는 `post_id` / `review_id` / `playlist_id` **nullable FK(exclusive-arc)**로 설계해 대상별 참조 무결성 유지
  * 알림 목록용 `(user_id, created_at DESC)`, 미읽음용 `(user_id, is_read, created_at DESC)` 등 빈번 조회 조건에 **SQL 복합 인덱스(B-Tree)** 수동 구축
  * 리뷰·플레이리스트 목록 조회 시 **ID를 선별한 뒤 `COUNT` / `GROUP BY` 집계를 분리**하고 필요 조인만 수행하도록 쿼리 구조 개선

* **외부 API 병렬화 및 이메일 OTP 인증 파이프라인 구축**
  * Spotify, iTunes, Odesli, Deezer 외부 API 조회를 `Promise.all`로 **서버사이드 병렬 처리**하고 **Next.js `unstable_cache` 및 TTL 캐시**로 반복 호출 최소화
  * **Resend** 연동으로 이메일 OTP 발송 파이프라인을 구축하고, **인증 코드 단방향 해시 저장 + 10분 TTL 만료** 정책을 적용해 회원가입 및 비밀번호 재설정 구현

* **Next.js App Router 기반 SEO 인프라 완성**
  * App Router 기반으로 사이트 전역 **메타데이터, Dynamic Open Graph(OG), robots.txt** 설정
  * 검색 엔진 크롤링 지원을 위해 주요 공개 경로를 수집하는 동적 **`sitemap.ts`** 구축 및 Vercel 프로덕션 운영

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
  * 컴포넌트 언마운트 시점에 **`removeEventListener` 클린업 함수**를 철저히 작성해 메모리 누수 원천 차단[cite: 1]

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
