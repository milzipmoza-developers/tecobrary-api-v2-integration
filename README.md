# Tecobrary Api v2 통합테스트를 위한 레포지토리 입니다.

<br>

## 프로젝트 종속성

> 해당 레포지토리는 다음 프로젝트들에 종속성을 가집니다.

1. 테코브러리 API server
    * 레포지토리 - [tecobrary-server-api-v2](https://github.com/milzipmoza-developers/tecobrary-server-api-v2)

2. 테코브러리 슬랙 알림 봇
    * 레포지토리 - [tecobrary-noti-slackbot](https://github.com/milzipmoza-developers/tecobrary-noti-slackbot)

3. 테코브러리 ELK
    * 레포지토리 - [tecobrary-elk](https://github.com/milzipmoza-developers/tecobrary-elk)    
<br>

## 레포지토리 목적

1. 프로젝트는 MSA 를 표방하여 서비스 별로 각각 다른 서버에서 동작합니다. 이를 통합테스트하기 위해 각 레포지토리에서 clone 을 하여 세팅을 해야하는데 이는 테스트에 불필요한 시간을 많이 투자해야 하기 때문입니다.

2. 추후 Milzipmoza OAuth 2 구축, 자동 배포 및 무중단 배포 등을 계획하고 있기 때문에 통합 테스트가 필수적입니다.

<br>

## 사용 방법

<br>

### 실행 관련 명령어

1. docker-compose 파일을 실행하는 명령어
```shell script
$ ELK_VERSION="7.5.0" docker-compose up -d
```
- ELK_VERSION : ELK 버전을 arg 로 입력해줘야 합니다.

<br>

2. docker-compose 실행을 종료하는 명령어
```shell script
$ docker-compose down
```

<br>

### 서브모듈 관련 명령어

1. 처음 레포지토리를 clone 했을 때 서브 모듈 안이 비어 있는 경우

```shell script
$ git submodule update --init --recursive
```

<br>
2. 서브 모듈을 추가하고 싶은 경우

```shell script
$ git submodule add [레포지토리 URL]
```
<br>
3. 서브 모듈을 업데이트 하고 싶은 경우

```shell script
$ git submodule update --remote
```