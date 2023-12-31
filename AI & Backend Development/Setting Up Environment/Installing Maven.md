# Maven

## Maven 이란?

* Java의 대표적인 빌드 툴(Build Tool) 중 하나
* apache 재단에서 개발하는 오픈소스 <https://maven.apache.org/>
* apache ant의 후속으로 개발
* XML을 사용하여 빌드 파일을 기술
* 중앙 저장소를 이용한 편리한 의존 관계 라이브러리 관리
* 중앙 저장소: 메이븐에서 이용 가능한 라이브러리를 모아서 관리하는 웹 서비스

## Maven의 장점

* 편리한 의존 관계 라이브러리 관리
* `일관된 디렉토리 구조와 빌드 프로세스 관리`
* `다양한 플러그인`

## Maven의 단점

* maven에서 기본적으로 지원하지 않는 빌드 과정 추가가 복잡해짐
* 플러그인의 설정이 상이하거나 장황해지면 재사용성 및 확장성이 떨어짐

# Maven 설치

## 다운로드 (직접 설치)

* <https://maven.apache.org/download.html>에서 maven 최신 버전을 다운받는다

## 설치 (Package Manager)

* Mac

```shell
brew install mvn
```

* Ubuntu

```shell
sudo apt update
sudo apt install maven
```

* Maven version check (설치확인)

```shell
mvn -version
```
