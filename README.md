# 👋 Hi, I'm bitedogo
### Full Stack Developer Based in Seoul

> **아이디어를 코드를 통해 현실로 만들어내는 과정에 몰입합니다.**
> <mark><b>확장성 있는 웹 애플리케이션</b></mark>과 <mark><b>안정적인 데이터 아키텍처</b></mark>를 설계하는 풀스택 개발자입니다.

[GitHub](https://github.com/bitedogo) · [Email](mailto:your.email@example.com) · [Instagram](https://instagram.com/your_id)

---

## 🚀 About Me

* **📍 Location:** 대한민국 서울
* **💻 Languages:** JavaScript, TypeScript, Java, Dart
* **🎯 Focus:** RESTful/Hybrid API 설계, 데이터베이스 최적화, 실시간 동기화 서비스 구현

---

## 🛠️ Technology Stack

### Languages & Frontend
<img src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/> <img src="https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript"/> <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=flat-square&logo=java&logoColor=white" alt="Java"/> <img src="https://img.shields.io/badge/dart-%230175C2.svg?style=flat-square&logo=dart&logoColor=white" alt="Dart"/> · <img src="https://img.shields.io/badge/Next.js-black?style=flat-square&logo=next.js&logoColor=white" alt="Next.js"/> <img src="https://img.shields.io/badge/react-%2320232a.svg?style=flat-square&logo=react&logoColor=%2361DAFB" alt="React"/> <img src="https://img.shields.io/badge/vue.js-%234FC08D.svg?style=flat-square&logo=vuedotjs&logoColor=white" alt="Vue.js"/> <img src="https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=flat-square&logo=tailwind-css&logoColor=white" alt="Tailwind CSS"/>

### Backend & Database
<img src="https://img.shields.io/badge/spring_boot-%236DB33F.svg?style=flat-square&logo=spring-boot&logoColor=white" alt="Spring Boot"/> <img src="https://img.shields.io/badge/node.js-6DA55F?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/> · <img src="https://img.shields.io/badge/supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" alt="Supabase"/> <img src="https://img.shields.io/badge/postgresql-%23316192.svg?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/> <img src="https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=oracle&logoColor=white" alt="Oracle"/> <img src="https://img.shields.io/badge/AWS_S3-569A31?style=flat-square&logo=amazons3&logoColor=white" alt="AWS S3"/>

### Tools
<img src="https://img.shields.io/badge/git-%23F05033.svg?style=flat-square&logo=git&logoColor=white" alt="Git"/> <img src="https://img.shields.io/badge/github-%23181717.svg?style=flat-square&logo=github&logoColor=white" alt="GitHub"/> <img src="https://img.shields.io/badge/vercel-%23000000.svg?style=flat-square&logo=vercel&logoColor=white" alt="Vercel"/> <img src="https://img.shields.io/badge/figma-%23F24E1E.svg?style=flat-square&logo=figma&logoColor=white" alt="Figma"/> <img src="https://img.shields.io/badge/intellij_idea-%23000000.svg?style=flat-square&logo=intellij-idea&logoColor=white" alt="IntelliJ IDEA"/> <img src="https://img.shields.io/badge/Visual_Studio_Code-007ACC?style=flat-square&logo=visual-studio-code&logoColor=white" alt="VS Code"/>

---

## 🎯 Featured Projects

### 💿 ORU (오루) — 음악 리뷰 및 소통 플랫폼
> 앨범 단위 평점 기록 및 음악 리스너 간의 취향 교감을 제공하는 풀스택 웹 서비스

* **기간:** 2025.10 ~ 현재 (진행 중)
* **기여:** 3인 팀 (본인 기여도: 개발 50%, DB 설계 30%)
* **기술:** `Next.js`, `TypeScript`, `Supabase`, `PostgreSQL`, `Vercel`
* **링크:** [Official Website](https://www.comeonoru.com) · [GitHub Repository](https://github.com/bitedogo/ourmusicreview)

**💡 기획 의도**
해외의 'RateYourMusic'이나 'Pitchfork'처럼 리스너들이 참여하는 음악 아카이브 및 리뷰 플랫폼이 국내에는 대중화되지 않았고, 기존 국내 전문 평론 매체들의 활성도가 낮다는 점에 주목했습니다. 이에 국내 대중음악 리스너들이 자유롭게 앨범 평점을 남기고 깊이 있는 감상을 공유할 수 있는 <mark><b>'사용자 참여형 음악 평론 커뮤니티 서비스'</b></mark>를 목적으로 기획 및 개발했습니다.

**🏗️ 기술 및 아키텍처 도입 배경**
* **Next.js (App Router):** 리뷰 게시글의 <mark><b>검색 엔진 최적화(SEO)</b></mark>를 확보하고, 다수의 외부 음원 API를 <mark><b>서버사이드에서 병렬로 호출</b></mark>하여 클라이언트 렌더링 부하를 줄이기 위해 도입했습니다.
* **Supabase & PostgreSQL:** 실시간으로 유저의 평점과 피드가 업데이트되는 커뮤니티 특성상, <mark><b>Realtime Subscription</b></mark> 기능과 강력한 관계형 데이터베이스를 함께 활용하여 백엔드 개발 생산성을 극대화했습니다.

**👨‍💻 핵심 성과**
* Next.js와 Supabase 기반의 음악 데이터 탐색 인프라 및 리뷰 CRUD API 전담 개발
* 유저 평점 및 피드 데이터를 실시간으로 집계하고 연동하는 결합 로직 구현
* NextAuth.js 기반 보안 환경 설계 및 Vercel 인프라 최적화로 지연 시간 최소화

<details>
<summary><b>🔥 트러블 슈팅 (클릭하여 펼치기)</b></summary>
<br>

| 이슈 | 문제 상황 | 해결 방안 | 결과 |
| :--- | :--- | :--- | :--- |
| **어뷰징 방어** | 무분별한 새로고침 및 매크로를 통한 조회수 조작 | 고유 키(IP+ID+게시글) 생성 및 분산 캐시(TTL 24시간) 검증 | 조작 0% 달성 및 부적절한 쓰기 쿼리 급감 |
| **API 병목 개선** | 외부 음원 API 순차 조회로 인한 렌더링 지연 | `Promise.all` 병렬 처리, 데이터 정규화 및 캐싱 도입 | 버튼 노출 속도 대폭 개선 및 네트워크 비용 절감 |

</details>

---

### 🐱 자바냥 (JavaNyang) — 온라인 자바 퀴즈 플랫폼
> 기초 문법부터 고급 개념까지 한 손으로 즐기는 웹/모바일 반응형 자바 프로필 학습 플랫폼

* **기간:** 2025.05 ~ 2025.07
* **기여:** 6인 팀 (Team Leader / 본인 기여도: DB 설계 40%, 개발 20%)
* **기술:** `React`, `Next.js`, `Supabase`, `PostgreSQL`, `Vite`
* **링크:** [Service Link](https://hyunsuplee.github.io/JavaNyang/) · [GitHub Repository](https://github.com/hyunsupLee/JavaNyang)

**💡 기획 의도**
딱딱하고 지루할 수 있는 프로그래밍 문법 학습에 <mark><b>'게이미피케이션(Gamification)'</b></mark> 요소를 결합하여 지속적인 학습 동기를 부여하고자 했습니다. 단순히 문제를 푸는 것을 넘어, 유저 간 실시간 1:1 대전과 업적 시스템을 통해 자바(Java)를 놀이처럼 재미있게 학습할 수 있는 생태계를 구축하는 것이 목적이었습니다.

**🏗️ 기술 및 아키텍처 도입 배경**
* **React:** 퀴즈 진행 및 대전 중 페이지 새로고침이 발생하지 않도록 <mark><b>SPA(Single Page Application)</b></mark> 형태로 구성하여 앱과 같은 부드러운 사용자 경험(UX)을 제공하고자 했습니다.
* **Supabase Realtime:** 별도의 복잡한 WebSocket 서버를 구축하고 유지보수하는 대신, BaaS의 실시간 채널 기능을 활용하여 <mark><b>저지연(Low-latency) 1:1 매칭</b></mark>과 양방향 라이브 채팅을 신속하고 안정적으로 구현했습니다.

**👨‍💻 핵심 성과**
* **팀 리딩:** 프로젝트 총괄 팀장으로서 애자일 일정 조율 및 관계형 데이터 구조 설계 주도
* 지속적인 학습 동기를 위한 난이도별 경험치 산정 및 실시간 업적 달성 게이미피케이션 엔진 설계
* Supabase Realtime 채널을 활용한 1:1 대전 매칭 및 양방향 라이브 채팅 개발

<details>
<summary><b>🔥 트러블 슈팅 (클릭하여 펼치기)</b></summary>
<br>

| 이슈 | 문제 상황 | 해결 방안 | 결과 |
| :--- | :--- | :--- | :--- |
| **화면 동기화 지연** | 다수 유저 실시간 대전 진입 시 전송 병목 및 싱크 어긋남 | 상태 구독 메타데이터 세분화 및 브로드캐스팅 주기 최적화 | 동시 접속 시 동기화 오차를 실시간 수준으로 압축 |

</details>

---

### 📚 StudyO (스터디오) — 올인원 스터디 협업 플랫폼
> 스터디 모집, 팀 빌딩, 체계적인 일정 관리 및 파일 공유를 지원하는 통합 관리 솔루션

* **기간:** 2025.07 ~ 2025.08 (5주)
* **기여:** 6인 팀 (본인 기여도: DB 설계 30%, 개발 20%)
* **기술:** `Java`, `Spring Boot`, `MyBatis`, `OracleDB`, `React`, `AWS S3`
* **링크:** [GitHub Frontend](https://github.com/hyunsupLee/react-study-o) · [GitHub Backend](https://github.com/hyunsupLee/tjspring)

**💡 기획 의도**
개발자나 취업 준비생들이 스터디를 운영할 때 소통은 메신저로, 자료는 클라우드로, 일정은 캘린더로 각각 파편화되어 진행되는 비효율에 주목했습니다. 팀 빌딩부터 목표 달성까지 필요한 모든 협업 기능을 한 곳에 모은 <mark><b>'올인원 스터디 워크스페이스'</b></mark>를 제공하여 학습과 협업의 마찰을 최소화하고자 기획했습니다.

**🏗️ 기술 및 아키텍처 도입 배경**
* **Spring Boot & OracleDB:** 다수의 유저 및 스터디 그룹 간의 <mark><b>복잡한 권한 처리(접근 제어)</b></mark>와 일정, 파일 등의 관계형 데이터를 안정적이고 무결성 있게 다루기 위해 엔터프라이즈급 생태계인 Spring Boot 환경을 채택했습니다.
* **AWS S3:** 스터디원들이 공유하는 대용량 학습 자료 및 이미지 파일들을 웹 서버(WAS) 부하 없이 <mark><b>안전하게 분산 저장</b></mark>하고 로드하기 위해 클라우드 스토리지를 연동했습니다.

**👨‍💻 핵심 성과**
* 유저별 참여 스터디 현황 및 주간 스케줄을 통합 시각화하는 비동기 데이터 대시보드 화면 구현
* 프로필 정보 및 이미지 업로드를 실시간으로 안전하게 처리하는 사용자 검증 모듈 구축
* 프론트엔드 코드 중복 감소 및 생산성 향상을 위한 전역 표준 모달(Modal) 아키텍처 설계

<details>
<summary><b>🔥 트러블 슈팅 (클릭하여 펼치기)</b></summary>
<br>

| 이슈 | 문제 상황 | 해결 방안 | 결과 |
| :--- | :--- | :--- | :--- |
| **렌더링 병목 현상** | 누적 일정 증가로 인한 캘린더 파싱 부하 및 프레임 드랍 | 쿼리 튜닝(필요 데이터만 추출) 및 디바운싱/useMemo 적용 | 프레임 드랍 제거 및 60fps에 준하는 렌더링 성능 확보 |

</details>

---
© 2026 bitedogo. All rights reserved.
