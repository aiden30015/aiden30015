# 이주언

### Flutter Developer

다음 사람이 이어받을 수 있는 앱을 만드는 Flutter 개발자입니다.
학교 기숙사와 외출제에서 실제로 쓰이는 앱 두 개를 운영하고 있습니다.

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white)

## 운영 중인 서비스

### Washer — 기숙사 세탁기 예약 앱

가입자 200명 이상, 일 평균 사용자 40명 · 2026.5 출시 후 운영 중

[App Store](https://apps.apple.com/kr/app/washer-v2/id6760886865) · [Google Play](https://play.google.com/store/apps/details?id=com.washer.v2) · [GitHub](https://github.com/team-washer/Washer-App-v2)

세탁기에 이름표를 걸어 순서를 잡던 방식을 대체한 앱입니다. 11명 팀의 앱 파트에서 예약 도메인과 배포 자동화를 맡았습니다.

- 예약 직전 재조회로 이미 예약된 기기를 걸러 내고, 연타는 기기별 single-flight로 병합
- 서버가 10분마다 갱신하던 기기 상태를, 조회 시점의 실제 상태를 보도록 변경
- main 머지 한 번으로 Android와 iOS 출시. 버전과 릴리스 노트를 검사하는 게이트와 인수인계 문서 포함

### GOMS — QR 기반 교내 외출 관리 앱

운영일(월, 수) 외출 인원 평균 100명 · 2026.2부터 운영 중

[Google Play](https://play.google.com/store/apps/details?id=com.goms.goms_android_v2) · [GitHub](https://github.com/team-haribo/GOMS-Android-V3)

학생회가 수기로 적던 외출 명단 관리를 QR 인증으로 대체했습니다. 이어받을 인원이 없던 Android 네이티브 앱을 Flutter로 다시 만들었습니다.

- 지도, QR 외출 인증, 인증과 토큰 처리 담당
- 앱을 켜 둔 동안 바뀐 권한이 반영되지 않던 문제를, 토큰 재발급 대신 프로필 재조회로 해결
- 직접 만든 성능 회귀 CI를 붙여 PR마다 관련 화면을 측정

## 오픈소스 / 도구

### thousands_separator_formatter

[pub.dev](https://pub.dev/packages/thousands_separator_formatter) · [GitHub](https://github.com/aiden30015/thousands_separator_formatter) · [Flutter PR #188243](https://github.com/flutter/flutter/pull/188243)

커서 위치 유지와 한글 조합 입력 보호를 지원하는 천 단위 구분 포매터입니다.
Flutter 이슈 [#188152](https://github.com/flutter/flutter/issues/188152)의 구현을 프레임워크 PR로 올렸고, "프레임워크가 의존하지 않는 독립 기능은 패키지로 두는 게 낫다"는 리뷰 의견을 받아 패키지로 배포했습니다. pub points 160/160.

### Flutter 성능 회귀 CI 파이프라인

[GitHub](https://github.com/aiden30015/Ci-App-Performance-Measurement) · [설계 문서](https://github.com/aiden30015/Ci-App-Performance-Measurement/blob/main/docs/DESIGN.md) · [대시보드](https://aiden30015.github.io/Ci-App-Performance-Measurement/)

앱이 느려진 걸 출시 후에야 알게 되는 문제를 막으려고, PR마다 주요 화면의 프레임, 메모리, 시작 시간을 재서 기준값과 비교하는 CI 도구를 만들었습니다. 측정 잡음을 MAD로 걸러 내고, 커밋별 추세를 대시보드로 남깁니다.

## 기술

**주력**

- Flutter, Dart — 운영 중인 앱 2개

**사용 경험**

- GitHub Actions, Fastlane — 스토어 자동 배포
- Firebase — FCM, Crashlytics
- Kotlin, Android XML — 네이티브 화면 구성
- Python — 코딩 테스트, 성능 CI 도구

## Contact

- Email: jueon.dev@gmail.com
- Blog: [velog.io/@aiden30015](https://velog.io/@aiden30015)
