# 1. 띵스플로우 github 권한 관리 규칙.
* Team 으로 구성 - 각 서비스 개발팀, 직무별 팀.
* 리포지토리를 수정해야 하는 직무군에 대해 Maintain 권한 부여.(ex : server)
* 리포지토리의 오너십을 가지는 직무군에 대해 admin 팀을 만들어 Admin 권한 부여.(ex : server-admin)
> admin 팀은 직무리드와, 직무리드 휴가시 대신할 수 있는 위임자로 구성합니다.
* 특정 서비스에 해당하는 리포지토리는 서비스 개발팀 전원에게 Read 권한 부여.(ex : storyplay)

# 2. 띵스플로우 github repository 명명 규칙.

|레벨1 : 서비스명|레벨2 : 직무명|레벨3(Optional) : 프로젝트명|
|------|---|---|
|between|iOS|chitchat|
|hellobot|android|design-system|
|storyplay|server|bankserver|
|platform|ai|product-server|
|common|web|   |
||ai|   |
||infra|   |
||data|   |
| |slack| |
| |temp| |
| |old| |

## 레벨1 설명.
  * between, hellobot, storyplay, platform : 서비스명.
  * common : 공통 모듈. 여러 서비스에서 가져다 쓰거나, 어느 서비스와도 관련이 없는 경우.
  * temp : 테스트 목적, 또는 임시 개발 목적으로 만드는 리포지토리. 
  * old : 소속이 분명하지 않고, 1년 이상 commit 기록이 없는 경우.
## 레벨3 설명
  * 3단계 명명은 의미를 쉽게 파악할 수 있게 합니다. 고유명사는 좋지 않습니다. 
  > storyplay-server-firefly(X)
  >
  > common-data-jupiter(X)
  >
  > storyplay-server-studio(O)

## 사용례
  * 스토리플레이 ios 앱
  > storyplay-iOS
  * 안드로이드 디자인 시스템 리포지토리
  > common-android-design-system
  * 헬로우봇 api 서버 
  > hellobot-server-mainapi
  * 인프라팀용 airflow 리포지토리(인프라팀 데이터 엔지니어가 관리하는) 
  > common-data-airflow
  * 스토리플레이 운영용 airflow 리포지토리(스플 서버 엔지니어가 관리하는) 
  > storyplay-server-airflow

***

###### 네이밍 규칙 변경에 대한 제안은 슬랙 #직무_개발 에서 @허인호 를 태그하여 주세요.
