# Tecobrary Api v2 통합테스트를 위한 레포지토리 입니다.

## 프로젝트 종속성

> 해당 레포지토리는 다음 프로젝트들에 종속성을 가집니다.

1. 테코브러리 API server
    * 레포지토리 - [tecobrary-server-api-v2](https://github.com/milzipmoza-developers/tecobrary-server-api-v2)

2. 테코브러리 슬랙 알림 봇
    * 레포지토리 - [tecobrary-noti-slackbot](https://github.com/milzipmoza-developers/tecobrary-noti-slackbot)
    
## 레포지토리 목적

1. 프로젝트는 MSA 를 표방하여 서비스 별로 각각 다른 서버에서 동작합니다. 이를 통합테스트하기 위해 각 레포지토리에서 clone 을 하여 세팅을 해야하는데 이는 테스트에 불필요한 시간을 많이 투자해야 하기 때문입니다.

2. 추후 Milzipmoza OAuth 2 구축, 자동 배포 및 무중단 배포 등을 계획하고 있기 때문에 통합 테스트가 필수적입니다.

 