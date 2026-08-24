<div align="center">

# 조경민
### 화면부터 데이터와 운영까지 연결하는 iOS · 백엔드 개발자

SwiftUI로 사용자가 믿을 수 있는 화면을 만들고,<br/>
Java와 Spring Boot로 데이터를 안정적으로 수집·저장·전달합니다.

[![iOS Portfolio](https://img.shields.io/badge/iOS_Portfolio-FA7343?style=flat&logo=notion&logoColor=white)](https://succulent-bamboo-7a2.notion.site/iOS-3c67ccd6244381239ce7df5ef952893a)
[![Backend Portfolio](https://img.shields.io/badge/Backend_Portfolio-6DB33F?style=flat&logo=notion&logoColor=white)](https://succulent-bamboo-7a2.notion.site/3c67ccd624438112aebac2c9186a3fdf)
[![Career Portfolio](https://img.shields.io/badge/Career_Portfolio-147EFB?style=flat&logo=notion&logoColor=white)](https://succulent-bamboo-7a2.notion.site/3c67ccd6244381f981edd56d387eaec5?pvs=74)
[![App Store](https://img.shields.io/badge/App_Store-0D96F6?style=flat&logo=appstore&logoColor=white)](https://apps.apple.com/kr/app/볼카운트/id6761362685)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:whrudals56@gmail.com)

</div>

---

## About

- iOS 화면, 상태 관리, 네트워크, 위젯, Live Activity와 푸시 알림을 구현하고 App Store에 직접 출시했습니다.
- 외부 데이터 수집부터 정규화, 저장, REST·SSE 전달, APNs와 운영 복구까지 백엔드 전체 흐름을 구축했습니다.
- 지연·누락·역순 응답에서도 정상 상태를 보존하도록 요청 세대, 상태 우선순위와 필드별 최신성을 함께 다룹니다.
- 운영 장애를 재현 가능한 테스트로 고정하고, 배포 전 반복 판단을 자동화합니다.
- 실무에서는 공공·기업 시스템의 기능 개발, DB 전환과 이관, 배포 검증, 고객 협의와 문서화를 수행했습니다.

## Tech Stack

### iOS

![Swift](https://img.shields.io/badge/Swift-FA7343?style=flat&logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0D96F6?style=flat&logo=swift&logoColor=white)
![Xcode](https://img.shields.io/badge/Xcode-147EFB?style=flat&logo=xcode&logoColor=white)

Observation · Swift Concurrency · URLSession · WidgetKit · ActivityKit · APNs · App Groups · Swift Testing

### Backend & Data

![Java](https://img.shields.io/badge/Java_17-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat&logo=springboot&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat&logo=hibernate&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=flat&logo=oracle&logoColor=white)

REST · SSE · Spring Scheduler · Flyway · MyBatis · JUnit

### Operations

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat&logo=gradle&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)

---

## Featured Project

### 볼카운트 — KBO 실시간 경기 정보 서비스

서로 다른 시점과 완성도로 도착하는 KBO 데이터를 하나의 현재 상태로 정리해 보여주는 개인 프로젝트입니다.<br/>
제품 방향, iOS 앱, 백엔드, 데이터베이스, 알림, 운영과 출시까지 전 과정을 직접 수행했습니다.

- [App Store에서 볼카운트 보기](https://apps.apple.com/kr/app/볼카운트/id6761362685)
- [iOS 소스 코드](https://github.com/rudadlswh/ballCount)
- [백엔드 소스 코드](https://github.com/rudadlswh/ballCount_back)

#### iOS

- SwiftUI와 Observation으로 홈, 순위, 일정, 경기 상세와 직관 기록 화면 구현
- 요청 세대, 상태 우선순위와 필드별 최신성을 이용해 지연·부분·역순 응답의 상태 역행 방지
- WidgetKit, ActivityKit, APNs와 App Groups를 연결해 앱 밖에서도 경기 상태 제공
- SSE 단절 시 REST 폴링으로 전환하고 연결 복귀 조건을 유지하는 복구 흐름 구성

#### Backend

- 외부 경기 데이터를 수집·파싱·정규화해 PostgreSQL에 경기 스냅샷과 이벤트로 저장
- 경기 상태에 따라 수집 주기를 조절하고, 해시와 이벤트 키로 중복 저장·알림 방지
- REST, SSE와 APNs의 역할을 분리해 조회·실시간 스트림·사용자 알림 제공
- Flyway 마이그레이션, 운영 콘솔, Docker와 환경별 설정 검증으로 운영 경계 구성

#### Quality & Release

- 지연, 빈 응답, 중복, 연결 실패와 복구 시나리오를 iOS·백엔드 자동화 테스트로 고정
- 운영 URL, 서명, 프로비저닝과 백엔드 설정을 확인하는 출시 전 검증 자동화
- iOS 앱을 App Store에 직접 출시하고 앱·서버 변경을 함께 관리

---

## Professional Experience

### 트루본 · 개발 및 운영 프로젝트

**2022.06 – 2025.06**

- 영화정보시스템에서 약 300개 테이블의 MS SQL → Oracle 전환과 전체 결과 검증
- 대법원 장비 도입 프로젝트에서 약 300만 건 규모의 Oracle 데이터 이관, 고객 협의와 문서화 수행
- 부과금 업무 신규 페이지 3개와 기존 기능 약 60건을 요구사항 분석부터 구현·검증까지 담당
- KTOA ITSM 전자서명 기능과 스마트초이스 모바일 화면 약 20개 개선
- 데이터 건수와 실제 업무 화면을 함께 점검하고 배포 이후 운영 동작까지 확인

[트루본 경력 포트폴리오 자세히 보기](https://succulent-bamboo-7a2.notion.site/3c67ccd6244381f981edd56d387eaec5?pvs=74)

---

## Portfolio

- [iOS 개발자 포트폴리오](https://succulent-bamboo-7a2.notion.site/iOS-3c67ccd6244381239ce7df5ef952893a)
- [백엔드 개발자 포트폴리오](https://succulent-bamboo-7a2.notion.site/3c67ccd624438112aebac2c9186a3fdf)
- [트루본 경력 포트폴리오](https://succulent-bamboo-7a2.notion.site/3c67ccd6244381f981edd56d387eaec5?pvs=74)

## Contact

- Email: [whrudals56@gmail.com](mailto:whrudals56@gmail.com)
