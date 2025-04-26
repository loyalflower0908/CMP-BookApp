# CMP-BookApp

**CMP-BookApp**은 Kotlin Multiplatform(코틀린 멀티플랫폼)을 활용하여 개발된 책 검색 애플리케이션입니다.  
외국 서적 검색 API를 이용해 다양한 책 정보를 조회할 수 있도록 구성되었습니다.

Android, iOS, Desktop 플랫폼을 동시에 지원하며, Ktor를 통한 API 통신과 Koin을 이용한 의존성 주입을 적용했습니다.  
Room Database도 구현을 시도했으나, iOS 플랫폼에서 NSFileManager 관련 이슈로 인해 중단된 상태입니다.

---

## 프로젝트 설명 🔍

CMP-BookApp은 하나의 코드베이스로 Android, iOS, Desktop을 모두 지원하는 Kotlin Multiplatform 프로젝트입니다.  
공통 비즈니스 로직과 UI를 최대한 공유하고, 각 플랫폼 특화 기능은 별도 모듈에서 처리하는 구조로 설계되었습니다.

외부 책 검색 API를 이용해 실시간으로 도서를 검색할 수 있으며, Ktor 기반의 네트워크 통신을 통해 빠르고 안정적인 데이터 교환을 지원합니다.

---

## 주요 기능 🚀

- **Kotlin Multiplatform 지원**
  - Android, iOS, Desktop을 단일 코드베이스로 관리
  - Compose Multiplatform을 통한 UI 구성

- **API 통신**
  - 외부 책 검색 API를 연동하여 도서 정보 검색
  - **Ktor Client**를 활용해 HTTP 요청 및 응답 처리

- **의존성 주입**
  - **Koin**을 사용해 ViewModel 및 Repository 등 주요 컴포넌트 관리

- **플랫폼별 코드 분리**
  - `commonMain` 폴더: 모든 플랫폼에서 공유되는 코드
  - `androidMain`, `iosMain`, `desktopMain`: 각 플랫폼 전용 코드

---

## 기술 스택 🧰

- **UI 및 멀티플랫폼 개발**
  - [Kotlin Multiplatform](https://kotlinlang.org/lp/mobile/)
  - [Compose Multiplatform](https://www.jetbrains.com/lp/compose-multiplatform/)

- **네트워크 통신**
  - [Ktor Client](https://ktor.io/docs/getting-started-ktor-client.html)

- **의존성 주입**
  - [Koin](https://insert-koin.io/)


---

## 참고 자료 📖

[Build a Clean Code Book App - Philipp Lackner](https://youtu.be/WT9-4DXUqsM?list=PLx76Utfso22Qf1wbc6phwDhAOgM6GLSY1)

---
