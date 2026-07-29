<div align="center">

# 조경민
### 데이터 흐름과 운영 안정성을 함께 설계하는 백엔드 개발자

Java·Spring Boot·PostgreSQL을 중심으로<br/>
외부 데이터 수집부터 저장, 실시간 전달, 장애 대응까지 서비스의 전체 흐름을 다룹니다.

</div>

---

## About

- 기능 구현에 그치지 않고 데이터 정합성, 예외 상황, 운영 안정성까지 함께 고려합니다.
- 로그·데이터베이스 상태·실행 흐름을 추적해 장애의 원인을 찾고 재발 방지 구조와 테스트로 연결합니다.
- 복잡한 요구사항을 작은 책임으로 나누고, 현재 규모에 맞는 단순하고 유지 가능한 설계를 지향합니다.
- Codex 등 AI 도구를 코드 분석과 테스트 작성에 활용하되, 변경 범위와 실행 결과를 직접 검증합니다.

## Tech Stack

### Backend

![Java](https://img.shields.io/badge/Java_17-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat&logo=springboot&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat&logo=hibernate&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat&logo=flyway&logoColor=white)

REST API · Spring Scheduler · SSE · APNs · OpenAPI

### Infrastructure & Testing

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat&logo=gradle&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)

JUnit 5 · Spring Boot Test · PostgreSQL Migration

### Additional Experience

![Swift](https://img.shields.io/badge/Swift-FA7343?style=flat&logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0D96F6?style=flat&logo=swift&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

---

## Featured Project

### 볼카운트 — KBO 실시간 경기 정보 서비스

KBO 경기 일정과 실시간 경기 상태를 수집·정제해 iOS 앱에 제공하는 개인 프로젝트입니다.  
백엔드, 데이터베이스, 실시간 전송, 알림, 운영 도구와 Docker 배포 환경을 직접 구축했습니다.

**Backend:** Java 17, Spring Boot 3.4, PostgreSQL, JPA, Flyway, Gradle  
**Client:** SwiftUI, WidgetKit, ActivityKit  
**Delivery:** SSE, APNs, Docker

#### 데이터 수집과 정합성

- 외부 경기 데이터를 파싱·정규화해 경기 스냅샷, 라인스코어, 선수 기록으로 저장
- 경기 전·진행 중·종료 후 상태에 따라 수집 주기를 조절하는 동기화 스케줄러 구현
- 원본 데이터 해시로 중복 저장을 줄이고, 이전·현재 상태 비교로 점수·출루·이닝 변화를 감지
- Flyway 마이그레이션과 환경별 스키마 분리로 개발·운영 데이터 변경 이력 관리

#### 실시간 기능과 운영

- SSE로 최신 경기 상태를 전달하고 APNs로 사용자별 팀·이벤트 설정에 맞는 알림 제공
- 이벤트 키 기반 중복 방지와 최신 요청 병합으로 반복 수집·알림 문제 개선
- 데이터 수집 상태와 오류 로그를 확인할 수 있는 운영 콘솔 구축
- 멀티 스테이지 Docker 이미지와 환경별 설정 검증으로 배포 과정의 실수를 줄임

#### 장애 대응 경험

데이터베이스 연결 오류가 스케줄러의 연쇄 실행을 중단시키는 문제를 로그와 실행 흐름으로 추적했습니다.  
예외가 발생해도 다음 동기화가 예약되도록 실행 구조를 보완하고, 재시도와 커넥션 풀 설정을 조정한 뒤 테스트로 회귀를 확인했습니다.

---

## AI-assisted Development

- Codex를 활용한 코드베이스 분석, 테스트 케이스 작성, 장애 로그 정리와 반복 작업 자동화
- AI가 제안한 변경은 기존 데이터 흐름과 영향 범위를 확인한 뒤 작은 단위로 적용
- 테스트와 실제 실행 결과를 기준으로 생성 코드의 정확성과 회귀 여부 검증

제가 생각하는 AI 시대의 백엔드 개발자는 구현 속도뿐 아니라,  
AI가 만든 결과의 위험을 판단하고 데이터 정합성·관측 가능성·복구 기준을 설계할 수 있어야 합니다.

---

## Contact

- Email: [whrudals56@gmail.com](mailto:whrudals56@gmail.com)
