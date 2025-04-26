코틀린 멀티플랫폼을 사용해서 만들어본 책 검색 앱.
외국 책 검색 API를 활용해서 만들었다.
코틀린 멀티플랫폼을 사용해서 만들어본 책 검색 앱.
외국 책 검색 API를 활용해서 만들었다.
API 통신은 Ktor로 구현했고 DI는 Koin을 사용하였다.
Room DB를 구현하다가 IOS 단에서 NSFileManager 부분에서 자꾸 오류가 나서... 아쉽지만 중간에 마무리를 하였다.

This is a Kotlin Multiplatform project targeting Android, iOS, Desktop.

* `/composeApp` is for code that will be shared across your Compose Multiplatform applications.
  It contains several subfolders:
  - `commonMain` is for code that’s common for all targets.
  - Other folders are for Kotlin code that will be compiled for only the platform indicated in the folder name.
    For example, if you want to use Apple’s CoreCrypto for the iOS part of your Kotlin app,
    `iosMain` would be the right folder for such calls.

* `/iosApp` contains iOS applications. Even if you’re sharing your UI with Compose Multiplatform, 
  you need this entry point for your iOS app. This is also where you should add SwiftUI code for your project.


Learn more about [Kotlin Multiplatform](https://www.jetbrains.com/help/kotlin-multiplatform-dev/get-started.html)…
