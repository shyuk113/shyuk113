<div align="center">

# 👋 안녕하세요, 백엔드 개발자 shyuk113입니다


> 도메인 중심 설계와 문제 해결을 즐기는 Java/Spring 백엔드 개발자입니다.

</div>

---

## 🛠 Tech Stack

<div align="center">

| 분류 | 기술 |
|------|------|
| **Language** | ![Java](https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white) |
| **Framework** | ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat&logo=springsecurity&logoColor=white) |
| **Database** | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white) |
| **ORM** | ![JPA](https://img.shields.io/badge/JPA-59666C?style=flat&logo=hibernate&logoColor=white) ![QueryDSL](https://img.shields.io/badge/QueryDSL-0769AD?style=flat) |
| **Tools** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white) |

</div>

---

## 📂 Projects

### 🛒 Home Shopping Backend
> Spring Boot 기반 홈쇼핑 백엔드 서버

- **기간**: 2025
- **기술**: Java 21, Spring Boot, Spring Security, JWT, JPA, Redis, MySQL
- **주요 구현**
  - JWT 기반 인증/인가 및 소셜 로그인
  - 비관적 락(`PESSIMISTIC_WRITE`)으로 재고 차감 동시성 문제 해결
  - Redis INCR 명령어의 원자성을 활용한 선착순 쿠폰 발급 시스템 구현
  - `@Transactional` + Redis 혼용 문제 해결 — 별도 서비스 클래스 분리로 트랜잭션 롤백 시 Redis 수동 롤백 처리
  - `@Cacheable` / `@CacheEvict`로 상품 조회 Redis 캐싱 적용
  - `GlobalExceptionHandler`로 도메인별 커스텀 예외 처리 및 적절한 HTTP 상태 코드 응답

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/shyuk113/home-shopping)

---

### 📚 Third Tool Backend
> 학습 카드(플래시카드) 관리 서비스 백엔드

- **기간**: 2025.09
- **기술**: Java 21, Spring Boot, Spring Security, JWT, JPA, QueryDSL, MySQL, Elasticsearch, AWS S3
- **팀 구성**: 백엔드 다수
- **담당 기능**
  - 태그별 월간 학습 통계 조회 API — `UserCardEntity → Card → Deck → Tag` JPQL 조인으로 학습 비율 집계 및 `Stats` BC 신규 구축
  - 덱 공유 라이브러리 기능 — 덱 공개/비공개 전환, 덱 복사(`originalDeck` 자기참조 관계 설계)
  - 다중 태그 AND 조건 검색 — 단일 태그에서 `List<Long>` 복수 태그 필터링으로 확장
  - 덱 이름 자동완성 — `LIKE :keyword%` JPQL + `Pageable`로 scope(공개/개인)별 최대 10개 결과 제한
  - `NameNormalizer` 유틸 도입 — NFKC 유니코드 정규화로 한글 자모 분리 문제 해결 및 대소문자 무시 태그 중복 방지
  - 태그 CRUD 서비스 레이어 테스트 코드 작성 (`TagControllerTest`, `TagServiceTest`)

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/Third-tool/third-tool-backend)

---

## 🔥 Problem Solving

<div align="center">

[![solved.ac profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=whitepaper113)](https://solved.ac/whitepaper113)

</div>

---

## 📊 GitHub Stats

<div align="center">

![shyuk113's GitHub stats](https://github-readme-stats.vercel.app/api?username=shyuk113&show_icons=true&theme=dark&hide_border=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=shyuk113&layout=compact&theme=dark&hide_border=true)

</div>

---

## 📫 Contact

<div align="center">

[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:danial25693@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/shyuk113)

</div>
