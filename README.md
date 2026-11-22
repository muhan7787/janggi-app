# 장기 (안드로이드 앱)

로그인, AI 대국, 승급 기능이 있는 장기 앱입니다. 게임 화면은 `app/src/main/assets/index.html` 하나에 모두 들어 있습니다.

## APK 만들기

### 방법 1. GitHub에서 자동으로 만들기 (PC 프로그램 설치 불필요)
1. github.com 에서 새 저장소(예: `janggi-app`)를 만듭니다.
2. 이 폴더의 파일을 모두 올립니다. (`.github` 폴더도 꼭 포함)
3. 저장소의 **Actions** 탭에서 "Build APK"가 끝날 때까지 기다립니다 (5분 정도).
4. 완료된 실행을 눌러 아래 **Artifacts**의 `janggi-apk`를 내려받고 압축을 풀면 `app-debug.apk`가 나옵니다.

### 방법 2. 윈도우 PC의 Android Studio로 만들기
1. Android Studio를 설치하고 이 폴더를 엽니다 (File > Open).
2. 동기화가 끝나면 Build > Build App Bundle(s) / APK(s) > Build APK(s).
3. `app/build/outputs/apk/debug/app-debug.apk`가 만들어집니다.

## 폰에 설치
1. `app-debug.apk`를 폰으로 옮겨 누릅니다.
2. "출처를 알 수 없는 앱 설치"를 허용하면 설치됩니다.

## 참고
- 계정과 승급 기록은 폰 안에만 저장됩니다. 앱을 지우면 기록도 사라집니다.
- 화면을 고치려면 `index.html`만 바꾸고 다시 빌드하면 됩니다.
