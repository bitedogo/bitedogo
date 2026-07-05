# 👋 Hi, I'm bitedogo
### Full Stack Developer Based in Seoul

> **아이디어를 코드를 통해 현실로 만들어내는 과정에 몰입합니다.**
> 확장성 있는 웹 애플리케이션과 안정적인 데이터 아키텍처를 설계하는 풀스택 개발자입니다.

[GitHub](https://github.com/bitedogo) · [Email](mailto:your.email@example.com)

---

## 🚀 About Me

* **📍 Location:** 대한민국 서울
* **💻 Languages:** JavaScript, TypeScript, Java, Dart
* **🎯 Focus:** RESTful/Hybrid API 설계, 데이터베이스 최적화, 실시간 동기화 서비스 구현

---

## 🛠️ Technology Stack

### Languages & Frontend
`TypeScript` `JavaScript` `Java` `Dart` · `Next.js` `React` `Vue.js` `Tailwind CSS`

### Backend & Database
`Spring Boot` `Node.js` · `Supabase` `PostgreSQL` `Oracle` `AWS S3`

### Tools
`Git` `GitHub` `Vercel` `Figma` `IntelliJ` `VS Code`

---

## 🎯 Featured Projects

### 💿 ORU (오루) — 음악 리뷰 및 소통 플랫폼
> **개발 기간:** 2025.10 ~ 현재 (진행 중)  
> **프로젝트 요약:** 앨범 단위 평점 기록 및 음악 리스너 간의 취향 교감을 제공하는 풀스택 웹 서비스  
> **참여도 & 인원:** 3명 (본인 기여도: 개발 50%, DB 설계 30%)  
> **Tech Stack:** `Next.js (App Router)`, `TypeScript`, `Supabase`, `PostgreSQL`, `Vercel`

#### 👨‍💻 담당 업무 및 핵심 성과
* **풀스택 아키텍처 구축:** Next.js와 Supabase 기반의 음악 데이터 탐색 인프라 및 리뷰 CRUD API 전담 개발
* **데이터 파이프라인 최적화:** 유저 평점 및 피드 데이터를 실시간으로 집계하고 연동하는 결합 로직 구현
* **인증 및 배포:** NextAuth.js 기반 보안 환경 설계 및 Vercel 인프라 최적화로 지연 시간 최소화

#### 📊 문제 해결 및 가치 입증 (Problem-Solving)
* **이슈 1: 무분별한 새로고침 및 본인 게시글 조회수 어뷰징 문제**
  * **문제 정의:** 사용자의 F5 연타나 본인 글 반복 클릭으로 트렌딩 게시글의 데이터 신뢰도가 떨어지고 서버 자원이 낭비되는 취약점 발견.
  * **가설 수립:** 클라이언트(세션)와 서버(작성자 검증)에서 2중 방어벽을 구축하면 유효 요청만 필터링하여 자원 소모를 최소화할 수 있을 것이다.
  * **액션 및 검증:** `sessionStorage`를 활용해 중복 요청을 1차 차단하고, API 단에서 로그인 세션 ID와 작성자 ID를 대조해 본인 조회는 카운트에서 제외하는 검증 로직 구현.
  * **결과 및 레슨:** 인위적 조회수 조작율 0% 달성. 데이터 신뢰성을 확보하며 방어적 설계의 중요성을 체득함.
* **이슈 2: 외부 음원 API 동시 호출 시 병목으로 인한 검색 성능 저하**
  * **문제 정의:** 다수의 공급사 API를 순차 호출(Waterfall)하면서 응답 속도가 지연되어 검색 UX가 저하되는 현상 발생.
  * **가설 수립:** 비동기 병렬 처리와 데이터 가공 레이어(Adapter)를 도입하면 응답 레이턴시를 단축하고 화면 안정성을 높일 수 있을 것이다.
  * **액션 및 검증:** `Promise.all` 기반 병렬 호출로 전환하고, 다형성 데이터를 표준 스펙으로 단일화하는 가공 레이어를 구축해 렌더링 비용 최적화.
  * **결과 및 레슨:** 검색 응답 속도 대폭 개선. 외부 데이터 소스를 안정적으로 제어하는 파이프라인 설계 역량 강화.

* **Links:** [Official Website](https://www.comeonoru.com) · [GitHub Repository](https://github.com/bitedogo/ourmusicreview)

---

### 🐱 자바냥 (JavaNyang) — 온라인 자바 퀴즈 플랫폼
> **개발 기간:** 2025.05 ~ 2025.07  
> **프로젝트 요약:** 기초 문법부터 고급 개념까지 한 손으로 즐기는 웹/모바일 반응형 자바 프로필 학습 플랫폼  
> **참여도 & 인원:** 6명 (Team Leader / 본인 기여도: DB 설계 40%, 개발 20%)  
> **Tech Stack:** `React`, `Next.js`, `Supabase`, `PostgreSQL`, `Vite`

#### 👨‍💻 담당 업무 및 핵심 성과
* **팀 리딩 & 데이터 모델링:** 프로젝트 총괄 팀장으로서 애자일 일정 조율 및 PostgreSQL 관계형 데이터 구조 설계 주도
* **게이미케이션 엔진 설계:** 지속적인 학습 동기를 위한 난이도별 경험치 산정 및 실시간 업적 달성 시스템 구축
* **실시간 인프라:** Supabase Realtime 채널을 활용한 1:1 대전 매칭 및 양방향 라이브 채팅 개발

#### 📊 문제 해결 및 가치 입증 (Problem-Solving)
* **이슈 1: 동시 다발적 대전 진입 시 클라이언트 간 화면 동기화 지연**
  * **문제 정의:** 대량의 유저가 실시간 대전에 진입할 때 정답 데이터 전송 병목이 일어나 타이머와 문제 출제 화면의 싱크가 어긋나는 치명적 결함 발생.
  * **가설 수립:** 전송 페이로드를 핵심 데이터 단위로 경량화하고 구독 범위를 세분화하면 네트워크 오버헤드가 해소될 것이다.
  * **액션 및 검증:** 전역 상태 구독을 최소한의 메타데이터 단위로 쪼개고, 브로드캐스팅 주기 최적화를 통해 클라이언트 패킷 크기 경량화.
  * **결과 및 레슨:** 동시 접속 시 동기화 오차 범위를 실시간 수준으로 압축하는 데 성공. 실시간 아키텍처에서 데이터 경량화가 성능에 미치는 직결적인 영향력을 학습함.

* **Links:** [Service Link](https://hyunsuplee.github.io/JavaNyang/) · [GitHub Repository](https://github.com/hyunsupLee/JavaNyang)

---

### 📚 StudyO (스터디오) — 올인원 스터디 협업 플랫폼
> **개발 기간:** 2025.07 ~ 2025.08 (5주)  
> **프로젝트 요약:** 스터디 모집, 팀 빌딩, 체계적인 일정 관리 및 파일 공유를 지원하는 통합 관리 솔루션  
> **참여도 & 인원:** 6명 (본인 기여도: DB 설계 30%, 개발 20%)  
> **Tech Stack:** `Java`, `Spring Boot`, `MyBatis`, `OracleDB`, `React`, `AWS S3`

#### 👨‍💻 담당 업무 및 핵심 성과
* **통합 대시보드 개발:** 유저별 참여 스터디 현황 및 주간 스케줄을 통합하여 시각화하는 비동기 데이터 대시보드 화면 구현
* **유효성 검사 및 비동기 처리:** 프로필 정보와 이미지 업로드를 실시간으로 안전하게 처리하는 사용자 검증 모듈 구축
* **공용 컴포넌트 표준화:** 프론트엔드 코드 중복을 줄이고 생산성을 높이기 위해 전역 표준 모달(Modal) 아키텍처 설계

#### 📊 문제 해결 및 가치 입증 (Problem-Solving)
* **이슈 1: 캘린더 내 대량의 일정 데이터 로딩 시 렌더링 병목 현상**
  * **문제 정의:** 누적 일정이 많아짐에 따라 fullCalendar 컴포넌트가 무거운 전체 데이터를 한 번에 파싱하면서 로딩이 지연되고 인터랙션 시 프레임이 끊기는 현상 발생.
  * **가설 수립:** 쿼리 단에서 불필요한 데이터 필드를 필터링하고, 프론트엔드의 불필요한 리렌더링 주기를 제어하면 60fps에 준하는 성능을 확보할 수 있을 것이다.
  * **액션 및 검증:** MyBatis 매퍼에서 필요한 데이터(일정명, 기간, ID)만 추출하도록 쿼리를 튜닝하고, 프론트엔드 단에서 `useMemo` 및 디바운싱을 적용해 상태 업데이트 빈도 제어.
  * **결과 및 레슨:** 스케줄 조작 시 발생하는 프레임 드랍을 제거하고 로딩 속도를 최적화함. 최적의 데이터 스펙 정의가 성능에 미치는 가치를 체득함.

* **Links:** [GitHub Frontend](https://github.com/hyunsupLee/react-study-o) · [GitHub Backend](https://github.com/hyunsupLee/tjspring)

---
© 2026 bitedogo. All rights reserved.
