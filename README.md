<div align="center">

# 조경민
### 실시간 데이터의 불완전함을 사용자가 믿을 수 있는 화면으로 바꾸는 iOS 개발자

SwiftUI를 중심으로 화면과 상태를 설계하고,<br/>
장애 경험을 테스트와 자동화 자산으로 남깁니다.

[![Portfolio](https://img.shields.io/badge/iOS_Portfolio-FF3B30?style=flat&logo=notion&logoColor=white)](https://succulent-bamboo-7a2.notion.site/iOS-3c67ccd6244381239ce7df5ef952893a)
[![App Store](https://img.shields.io/badge/App_Store-0D96F6?style=flat&logo=appstore&logoColor=white)](https://apps.apple.com/kr/app/볼카운트/id6761362685)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:whrudals56@gmail.com)

</div>

---

## About

- 사용자가 지금 필요한 정보를 빠르게 파악하도록 화면의 정보 우선순위와 상태별 표현을 설계합니다.
- 지연·누락·역순 응답에서도 정상 상태를 보존하도록 요청 세대, 상태 우선순위와 필드별 최신성을 함께 다룹니다.
- 앱, 위젯, Live Activity와 푸시 알림이 동일한 상태 규칙을 공유하도록 구현합니다.
- 문제를 재현 가능한 테스트로 고정하고, 배포 전 반복 판단은 자동화합니다.
- 백엔드와 데이터베이스까지 직접 구현한 경험을 바탕으로 앱과 서버 사이의 경계를 함께 이해합니다.

## Tech Stack

### iOS

![Swift](https://img.shields.io/badge/Swift-FA7343?style=flat&logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0D96F6?style=flat&logo=swift&logoColor=white)
![Xcode](https://img.shields.io/badge/Xcode-147EFB?style=flat&logo=xcode&logoColor=white)

Observation · Swift Concurrency · URLSession · WidgetKit · ActivityKit · APNs · Swift Testing

### Backend & Operations

![Java](https://img.shields.io/badge/Java_17-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat&logo=springboot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

REST · SSE · Flyway · JUnit · GitHub Actions

---

## Featured Project

### 볼카운트 — KBO 실시간 경기 정보 iOS 앱

서로 다른 시점과 완성도로 도착하는 KBO 데이터를 하나의 현재 상태로 정리해 보여주는 개인 프로젝트입니다.<br/>
제품 방향, iOS 앱, 백엔드, 데이터베이스, 알림과 출시까지 전 과정을 직접 수행했습니다.

- [App Store에서 볼카운트 보기](https://apps.apple.com/kr/app/볼카운트/id6761362685)
- [iOS 소스 코드](https://github.com/rudadlswh/ballCount)
- [iOS 개발자 포트폴리오](https://succulent-bamboo-7a2.notion.site/iOS-3c67ccd6244381239ce7df5ef952893a)

#### 신뢰할 수 있는 실시간 상태

- 늦게 도착한 예정 응답이 라이브·종료 상태를 덮지 않도록 상태 병합 정책 구현
- 부분·빈 응답이 기존 정상 값을 삭제하지 않도록 필드별 최신성과 출처 우선순위 적용
- SSE 단절 시 REST 폴링으로 전환하고 연결 복귀 조건을 유지하는 복구 흐름 구성

#### Apple 플랫폼 경험

- SwiftUI와 Observation을 이용해 홈, 순위, 일정과 경기 상세 화면 구현
- WidgetKit, ActivityKit과 APNs를 연결해 앱 밖에서도 경기 상태 제공
- App Groups를 이용해 앱, 위젯과 Live Activity가 상태 규칙과 데이터를 공유하도록 구성

#### 품질과 출시

- 지연, 빈 응답, 중복과 연결 실패를 자동화 테스트의 회귀 조건으로 고정
- 운영 URL, 서명, 프로비저닝과 백엔드 설정을 확인하는 출시 전 검증 자동화
- App Store에 직접 출시하고 실제 운영에 필요한 앱·서버 경계를 함께 관리

---

## Contact

- Email: [whrudals56@gmail.com](mailto:whrudals56@gmail.com)
- Portfolio: [iOS 개발자 포트폴리오](https://succulent-bamboo-7a2.notion.site/iOS-3c67ccd6244381239ce7df5ef952893a)
