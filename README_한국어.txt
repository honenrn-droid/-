TBN 제주 라디오 앱 프로젝트

구성
- 한국어 화면
- 어르신이 보기 쉽도록 큰 글자와 큰 버튼
- TBN 제주교통방송(FM 105.5MHz) 안내
- 공식 TBN 홈페이지를 앱 안에서 열어 실시간 방송을 듣는 방식

중요
현재 공식 사이트의 온에어 화면은 지역 선택형입니다. 이 프로젝트는 공식 사이트를 열며,
실제 재생 화면에서 '제주' 지역을 선택해야 할 수 있습니다.
방송사의 공식 스트리밍 주소가 공개적으로 고정 확인되지 않아 임의 주소를 넣지 않았습니다.

APK 만들기
1. PC에 Android Studio를 설치합니다.
2. Android Studio에서 'Open'을 누르고 이 압축을 푼 TBN_Jeju_Radio_Android 폴더를 엽니다.
3. Gradle 동기화가 끝날 때까지 기다립니다.
4. 메뉴 Build > Build Bundle(s) / APK(s) > Build APK(s)를 선택합니다.
5. 완료 알림의 'locate'를 누르면 app-debug.apk 파일을 찾을 수 있습니다.
6. 휴대폰으로 APK를 옮겨 설치합니다. 설치 시 '알 수 없는 앱 설치 허용'이 필요할 수 있습니다.

공식 방송 안내: https://www.tbn.or.kr/
제주 주파수: FM 105.5MHz


[PC 없이 온라인에서 APK 만들기 - GitHub Actions]
1. 휴대폰 브라우저에서 https://github.com 에 가입/로그인합니다.
2. 새 저장소(New repository)를 만듭니다. 이름은 TBN-Jeju-Radio, Public 또는 Private 아무거나 가능합니다.
3. 저장소 화면에서 Add file > Upload files를 누릅니다.
4. 이 ZIP의 압축을 풀고, 안에 있는 모든 파일과 .github 폴더를 저장소에 업로드합니다.
   (ZIP 파일 자체를 올리는 것이 아니라 압축을 푼 파일들을 올려야 합니다.)
5. Commit changes를 누릅니다.
6. 저장소의 Actions 탭 > Build Android APK > Run workflow를 누릅니다.
7. 작업이 초록색 체크로 끝나면 해당 실행 결과 페이지 아래 Artifacts에서
   TBN-Jeju-Radio-APK를 눌러 다운로드합니다.
8. 다운로드한 ZIP을 풀면 app-debug.apk가 있습니다. APK를 눌러 설치합니다.
9. 설치가 막히면 휴대폰 설정에서 해당 브라우저/파일 앱의 '알 수 없는 앱 설치 허용'을 켭니다.

참고: GitHub 계정과 인터넷 연결이 필요합니다. GitHub Actions의 무료 사용량/정책에 따라
빌드가 제한될 수 있습니다. APK는 테스트용(debug) 서명 APK입니다.
