<div align="center">

# 안녕하세요, 김용빈입니다 👋

**설계부터 배포·운영까지 끝까지 책임지는 풀스택(백엔드 중심) 개발자를 지향합니다**

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=16&pause=1200&color=6366F1&center=true&vCenter=true&width=520&lines=Full-stack+%C2%B7+Backend-focused;TypeScript+%7C+NestJS+%7C+PostgreSQL;Java+%7C+Spring+Boot;Ship%2C+measure%2C+review%2C+repeat)](https://git.io/typing-svg)

</div>

---

### 🃏 Featured — Pokémon Card Dex

<div align="center">

**포켓몬 카드 20,635장을 한국어로 검색하고, 영문·일본·PSA 시세를 원화로 보고, 덱을 짜고, 가상 포인트로 경매하는 서비스**

[![Live](https://img.shields.io/badge/Live-pokemon--card--dex-e3350d?style=for-the-badge&logo=vercel&logoColor=white)](https://pokemon-card-dex-green.vercel.app) [![Repo](https://img.shields.io/badge/Repo-pokemon--cardgame-24292f?style=for-the-badge&logo=github)](https://github.com/Yongb15/pokemon-cardgame) [![Release](https://img.shields.io/github/v/release/Yongb15/pokemon-cardgame?style=for-the-badge&color=6366F1)](https://github.com/Yongb15/pokemon-cardgame/releases)

<img src="https://raw.githubusercontent.com/Yongb15/pokemon-cardgame/main/docs/screenshots/demo.gif" width="720" alt="검색 → 카드 상세 → 시세 순위 → 경매"/>

</div>

| 항목 | 내용 |
|---|---|
| **규모** | 카드 20,635장 · 세트 176개 · 하루 약 4천 장 시세 자동 수집 · 릴리스 v1.0 → v1.7 (2026-10) |
| **구조** | React 19 SPA (Vercel) → Vercel Functions(카드·시세) / NestJS on Cloud Run(계정·경매) → Neon PostgreSQL · Cloud Run Job 수집기 |
| **동시성** | 가상 포인트 경매 — 추가만 하는 포인트 장부, 전역 잠금 순서로 **50건 동시 입찰 교착 0건**, 마감 연장·지연 정산 |
| **보안** | OIDC + PKCE 소셜 로그인, `__Host-` 세션, 테이블·컬럼 단위 최소 권한 DB 계정 3개, 관리자 404·12시간 재로그인 |
| **품질** | Vitest 300여 개 + 실제 Postgres 동시성 점검 스크립트, Lighthouse 접근성·권장사항·SEO 100, 단계마다 qa·보안 리뷰 |
| **문제 해결** | 절반 실패하던 수집기 → 오류 라벨로 `53300 too many connections` 추적 후 풀러 전환(실패 0) · 이름이 다른 일본판 카드를 **그림 해시**로 대조 |

<p align="center"><a href="https://github.com/Yongb15/pokemon-cardgame#구조">🧭 구조도</a> &nbsp;·&nbsp; <a href="https://github.com/Yongb15/pokemon-cardgame#문제-해결-기록">🔧 문제 해결 기록</a> &nbsp;·&nbsp; <a href="https://github.com/Yongb15/pokemon-cardgame/releases">📦 릴리스 노트</a></p>

---

### 🛠 Tech Stack

<div align="center">

**Frontend** &nbsp; ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)

**Backend** &nbsp; ![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)

**Data** &nbsp; ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Drizzle](https://img.shields.io/badge/Drizzle_ORM-C5F74F?style=flat-square&logo=drizzle&logoColor=black) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**Infra** &nbsp; ![Google Cloud](https://img.shields.io/badge/Cloud_Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

**Also** &nbsp; ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

</div>

---

### 📌 Projects

| 프로젝트 | 설명 | 스택 |
|---|---|---|
| 🃏 [**Pokémon Card Dex**](https://github.com/Yongb15/pokemon-cardgame) | 카드 도감·시세·덱 빌더·가상 포인트 경매 풀스택 서비스 ([사이트](https://pokemon-card-dex-green.vercel.app)) | React · TypeScript · NestJS · PostgreSQL · GCP |
| 🎮 [QMatch](https://github.com/Yongb15/QMatch) | 게임 유저 매칭 플랫폼 (2025 졸업작품) | Spring Boot · React · Electron · WebSocket |
| 🛡 [Jailbreak](https://github.com/Yongb15/Jailbreak) | 한국어 페르소나 기반 Jailbreak 공격에 대한 LLM 보안 성능 비교 연구 | Python · Prompt Engineering |
| 🎲 [WindowAPI_YutNori](https://github.com/Yongb15/WindowAPI_YutNori) | C++ Windows API 기반 윷놀이 게임 | C++ · Windows API |
| 📒 [Ref_GuestBook](https://github.com/Yongb15/Ref_GuestBook) | 방명록 (파일 입출력 · 메모리 관리) | C++ |
| 🧩 [OOP-Study](https://github.com/Yongb15/OOP-Study) | C# 객체지향 설계 스터디 | C# |

---

<table>
<tr>
<td valign="top" width="50%">

### 🎓 Education

| 기간 | 내용 |
|---|---|
| 2023 – 2025 | 유한대학교 컴퓨터소프트웨어공학과 졸업 |
| 2026 – 2027 | 유한대학교 컴퓨터소프트웨어공학과 전공심화 재학 중 |

</td>
<td valign="top" width="50%">

### 📜 Certifications

| 자격증 | 발급처 |
|---|---|
| 정보처리산업기사 | 한국산업인력공단 |
| 리눅스마스터 2급 | 한국정보통신진흥협회 |
| 전기기능사 | 한국산업인력공단 |
| 승강기기능사 | 한국산업인력공단 |

</td>
</tr>
</table>

---

### 📊 Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Yongb15&show_icons=true&theme=tokyonight&hide_border=true&border_radius=8&rank_icon=github" height="150"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Yongb15&layout=compact&theme=tokyonight&hide_border=true&border_radius=8" height="150"/>

</div>

---

<div align="center">

📫 dydqls5658@naver.com &nbsp;·&nbsp; [Notion 포트폴리오](https://app.notion.com/p/378ef01e202b806f92efdbf647126682)

</div>
