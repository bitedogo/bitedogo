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

| 영역 | 기술 스택 |
| :--- | :--- |
| **Frontend** | `TypeScript` `JavaScript` `Next.js` `React` `Vue.js` `Tailwind CSS` `Dart` |
| **Backend & DB** | `Java` `Spring Boot` `Node.js` `Supabase` `PostgreSQL` `OracleDB` `TypeORM` `AWS S3` |
| **Tools & AI** | `Git` `GitHub` `Cursor AI` `Vercel` `IntelliJ IDEA` `VS Code` |

---

## 🎯 Featured Projects

### 💿 ORU (오루) — 음악 리뷰 및 아카이빙 플랫폼
> **"국내 대중음악 리스너를 위한 앨범 단위 평점 & 아카이빙 웹 서비스"**

| 구분 | 상세 내용 |
| :--- | :--- |
| **Period** | 2025.10 ~ 현재 (프로덕션 운영 중) |
| **Team / Role**| 3인 팀 (`기획 100%`, `풀스택 개발 50%`, `DB 설계 30%`) |
| **Tech Stack** | `Next.js (App Router)` `TypeScript` `Supabase` `PostgreSQL` `TypeORM` `Vercel` |
| **Links** | [🌐 서비스 링크 (comeonoru.com)](https://www.comeonoru.com) &nbsp;\|&nbsp; [📦 GitHub Repo](https://github.com/bitedogo/ourmusicreview) |

#### 🔧 Key Engineering & Problem Solving

* **외부 음원 API 병렬화 및 캐싱 파이프라인 구축**
  * **Problem:** Spotify, iTunes, Deezer 등 다중 외부 음원 API를 순차 호출하면서 응답 지연 발생
  * **Solution:** `Promise.all` 기반 서버사이드 병렬 호출 및 캐싱 로직 적용
  * **Result:** 네트워크 Latency 최소화 및 앨범 스트리밍 링크 렌더링 체감 속도 개선

* **조회수 중복 집계 방지 및 불필요한 DB 쓰기 완화**
  * **Problem:** 무분별한 새로고침 및 본인 작성 글 열람 시 불필요한 `UPDATE` 쿼리 빈번 발생
  * **Solution:** 세션 키 기반 조회 검증 인터셉트 및 작성자 식별 필터링 구현
  * **Result:** 비정상적 트래픽에 의한 데이터 왜곡 방지 및 DB 부하 절감

* **검색 엔진 최적화(SEO) 및 프로덕션 운영 안정화**
  * **Implementation:** Next.js Server Component 구조화, Dynamic OG 메타태그 및 Sitemap 파이프라인 세팅
  * **Impact:** 앨범·리뷰 페이지의 검색 엔진 수집 최적화 및 Vercel 실서버 무중단 배포 환경 확립

---

### 🐱 자바냥 (JavaNyang) — 실시간 자바 퀴즈 배틀 플랫폼
> **"게이미피케이션 요소와 1:1 라이브 대전을 결합한 자바 학습 웹 서비스"**

| 구분 | 상세 내용 |
| :--- | :--- |
| **Period** | 2025.05 ~ 2025.07 |
| **Team / Role**| 6인 팀 (`Team Leader & PM`, `DB 설계 40%`, `개발 20%`) |
| **Tech Stack** | `React` `Next.js` `Supabase Realtime` `PostgreSQL` `Vite` |
| **Links** | [🌐 서비스 체험 (GitHub Pages)](https://hyunsuplee.github.io/JavaNyang/) &nbsp;\|&nbsp; [📦 GitHub Repo](https://github.com/hyunsupLee/JavaNyang) |

#### 🔧 Key Engineering & Problem Solving

* **Supabase Realtime 기반 대전 상태 Pub/Sub 아키텍처 설계**
  * **Problem:** 다중 라운드 1:1 대전 시 방 상태, 참가자 레디, 답안 제출 간 상태 동기화 누락 위험
  * **Solution:** `postgres_changes` 구독 채널을 방 단위/라운드 단위로 관심사 분리(Pub/Sub)
  * **Result:** 5라운드 실시간 대전 진행 간 답안 제출 및 점수 판정 데이터 유실 없이 안정적 동기화

* **학습 지속성을 위한 게이미피케이션 시스템 구축**
  * **Implementation:** 퀴즈 채점 결과에 따른 실시간 EXP 적립 및 레벨 계산 로직 개발
  * **Impact:** 출석·정답 수 조건의 업적(`achievements`) 테이블 트리거 및 실시간 리더보드 연동으로 재도전 루프 완성

* **스프린트 리딩 및 기한 내 릴리즈**
  * **Implementation:** 요구사항 정의, 데이터 모델링 주도, 컴포넌트 단위 인터페이스 규격화
  * **Impact:** 기획 단계 스펙(퀴즈/대전/채팅/업적)을 스프린트 일정 내 100% 구현 및 배포 완료

---

### 📚 StudyO (스터디오) — 올인원 스터디 협업 플랫폼
> **"스터디 모집부터 일정 관리, 자료 공유를 통합한 협업 워크스페이스"**

| 구분 | 상세 내용 |
| :--- | :--- |
| **Period** | 2025.07 ~ 2025.08 (5주) |
| **Team / Role**| 6인 팀 (`프론트엔드 개발 20%`, `DB 모델링 30%`) |
| **Tech Stack** | `Java` `Spring Boot` `MyBatis` `OracleDB` `React` `AWS S3` |
| **Links** | [📦 Frontend Repo](https://github.com/hyunsupLee/react-study-o) &nbsp;\|&nbsp; [📦 Backend Repo](https://github.com/hyunsupLee/tjspring) |

#### 🔧 Key Engineering & Problem Solving

* **React Portal 기반 공통 모달 프리셋 시스템화**
  * **Problem:** 화면마다 반복되는 확인/알림 모달 구현으로 인한 코드 중복 및 UI 불일치
  * **Solution:** Confirm/Alert/Action 타입별 프리셋을 정의한 재사용 전역 Portal 컴포넌트 설계
  * **Result:** 마이페이지 및 멤버 관리 전역의 모달 작성 공수 단축 및 사용자 인터랙션 통일

* **다중 스터디 일정 데이터 비동기 병렬화**
  * **Problem:** 참여 스터디가 많을수록 마이페이지 내 캘린더 일정 조회 요청이 누적되어 병목 발생
  * **Solution:** 다중 일정 API 비동기 병렬 호출 및 날짜별 단일 이벤트 매핑 구조 간소화
  * **Impact:** 캘린더 UI 렌더링 딜레이 제거 및 `useMemo` 기반 호스트 권한 분리로 일정 조작 무결성 확보

* **사전 검증 기반 클라이언트 파일 업로드 파이프라인**
  * **Implementation:** 브라우저 단에서 이미지 확장자 선별 및 용량 제한 선검증 후 `FormData` 전송
  * **Impact:** 비정상 파일 전송으로 인한 서버 낭비를 막고, AWS S3 경로 연동으로 미디어 서빙 분리

---

<p align="center">
  © 2026 <b>bitedogo</b>. Built with passion & clean architecture.
</p>
