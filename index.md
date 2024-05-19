---
title: Home
layout: home
---

# 데이터 베이스 선택의 기준
* 무결성이 필요한 금융 서비스에는 관계형 데이터베이스를 사용하고, 
* 실시간 입찰이나 온라인 쇼핑 등에는 키-밸류 기반 NoSQL,
* 문서 형태의 저장이 필요한 컨텐트 관리및 모바일 서비스를 위한 도큐멘트 데이터베이스,
* 캐싱및 실시간 분석을 위한 인메모리 데이터베이스,
* 데이터간 관계 분석을 위한 그래프 디비,
* 시간에 따른 데이터를 수집하고 분석하는 시계열 디비,
* 원본데이터의 변경을 막는 블럭체인 기반의 원장 데이터베이스

![](/images/datastore/목적에맞는데이터베이스사용과현대화.png)
![](/images/datastore/usecases-01.png)

# Migration Tools
DB 스키마 관리, 마이그레이션 관련 소프트웨어를 정리한다.

# Flyway
rdb database migration

Spring 에서 db schema 관리를 해주는 툴

* 만약에 flyway와 ddl-auto: true가 동시에 적용되있으면, flyway가 먼저 동작하는 걸 확인함.

# Liquidate
KeyCloack이 사용하고 있는 migration tool


# Columnar Database
* 대량의 데이터를 이용하는 경우에 사용하게 된다.
* 조회 성능이 탁월하고, 
* 업데이트 성능은 낮은 특성을 가진다.

* 데이터 분석시에 매우 유용하다.

* 많이 사용되는 사례로 채팅 메세지를 저장하는 용도로 사용된다.
  + 예. Discord


# Bad Relational Database

* 배너 정보를 저장하는 테이블 스키마를 고민하다가 든 생각
mongodb가 많이 사용되는 유스케이스를 살펴보자. json 형태로 데이터를 free하게 세팅할 수 있을거 같다. 하지만, 만약에 mongodb도 스키마 세팅을 해야지 사용해야하는 Feature가 있지않은가? ElasticSearch 같은 경우는 Schema를 세팅해야지 사용할 수 있는 기능이 많았던거 같다.


# Sharding RDB
[우아한형제들 DB분산처리를 위한 sharding](https://techblog.woowahan.com/2687/)
 
=> Spring을 활용한 현실적인 가이드
 
 
 
[실무에서 DB를 샤딩할 때 주로 어떤 DB를 사용하나요?](https://okky.kr/articles/1313183)

=> MySQL보다 MongoDB???
 


### vitess
https://vitess.io/
  
youtube에서 사용하는 오픈소스 솔루션
 
 
 
### shardingsphere
https://shardingsphere.apache.org/ 
 
아파치에서 개발하는 오픈 소스 

