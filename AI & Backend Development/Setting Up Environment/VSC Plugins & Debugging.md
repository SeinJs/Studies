# VSCode PlugIn

## (필수) Extension Pack for Java

## (필수)Sonarlint
- 코딩 문제를 해결할 수 있도록 도와주는 무료 IDE 확장 프로그램. 
- 코드를 작성하는 동안 버그, 취약점 및 코드 향기로 이어질 수 있는 문제를 감지하고 강조 표시합니다.

## TODO Tree
- TODO나 FIXME 등의 주석을 찾아 를 트리 형태로 보여주는 플러그인

## Korea Language Pack for Visual Studio Code
- VSCode를 한국어 버전으로 보여주는 확장 프로그램

## Material Theme
- VSCode 테마를 바꿀 수 있도록 해주는 플러그인

## Rainbow Brackets
- 중괄호 {}의 색을 변경해주는 플러그인

# Debugging Tool

### [Debugging][^debug]이란?
- 컴퓨터 프로그램 개발 단계 중에 발생하는 시스템의 논리적 오류나 비정상적인 연산(버그)을 찾아내 그 원인을 밝히고 수정하는 작업 과정
- Debugger : 디버깅을 돕는 도구

## Visual Studio Code의 Debugger
- VSCode 왼쪽 상단의 Run and Debug 또는 오른쪽 상단 Debug Java 눌러 디버깅 가능

![Run and Debug](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/debugging1.png)
![Debug Java](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/debugging2.png)

## Break point
- 프로그램을 의도적으로 멈추게 하는 장소
- 디버깅을 목적으로 break point를 설정하며, 이를 통해 내부의 다양한 값들을 확인하며 프로그램을 분석 & 검증할 수 있음

## debug 관련 기능

![Debugger](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/debugger.png)

1. `continue`(F5) -> 다음 break point를 만날때까지 계속 진행
2. `Step Over`(F10) -> 한 줄 실행
3. `Step Into`(F11) -> 함수 내부로 들어감
4. `Step Out`(shift+F11) -> 함수를 끝까지 실행시키고 호출시킨 곳으로 되돌아감 
5. `Restart`(ctrl+shift+F5) -> 재시작 
6. `Stop`(shift+F5) -> 디버깅 중지
7. `Hot Code Replace` -> 자바용 디버거 동작 중에 새로운 클래스 파일의 변경이 있으면 그 변경된 파일을 자동으로 교체하는 디버깅 기술

[^debug]: https://ko.wikipedia.org/wiki/%EB%94%94%EB%B2%84%EA%B7%B8
