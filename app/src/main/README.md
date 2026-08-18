# 시호의 머니노트 - Android App

이 프로젝트는 브라우저용 PWA가 아니라 **실제 Android 앱 프로젝트**입니다.

## 핵심
- 앱 이름: 시호의 머니노트
- 패키지: com.siho.moneynote
- 화면: 기존 `시호의 머니노트 V4`를 앱 내부에 번들
- 인터넷 없이 기본 계산 기능 사용 가능
- 입력값은 Android WebView의 로컬 저장소에 보관
- 은행 계좌 연동/실제 이체 기능 없음
- `content://downloads`에서 HTML을 여는 방식이 아님

## APK 만들기
GitHub에 이 프로젝트를 올리면 `.github/workflows/build-apk.yml`이 자동으로 APK를 빌드합니다.
Actions 실행 결과의 `SihoMoneyNote-APK` artifact 안에 `app-debug.apk`가 생성됩니다.

또는 Android Studio에서 프로젝트를 연 뒤:
Build > Build APK(s)

## 빌드 사양
- Android Gradle Plugin 8.7.3
- Gradle 8.9
- compileSdk 35
- targetSdk 35
- minSdk 23
- Java 17
