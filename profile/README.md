# 띵스플로우 github repository 명명 규칙.

|레벨1 : 서비스명|레벨2 : 직무명|레벨3(Optional) : 프로젝트명|
|------|---|---|
|between|ios|chitchat|
|hellobot|android|design-system|
|storyplay|server|bankserver|
|common|web|   |
|temp|sre|   |
|old|data|   |
| |slack| |

## 레벨1 설명.
  * between, hellobot, storyplay : 서비스명.
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
  > storyplay-ios
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
