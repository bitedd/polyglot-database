---
title: Home
layout: home
---

# Migration Tools
DB 스키마 관리, 마이그레이션 관련 소프트웨어를 정리한다.

# Flyway
rdb database migration

Spring 에서 db schema 관리를 해주는 툴

* 만약에 flyway와 ddl-auto: true가 동시에 적용되있으면, flyway가 먼저 동작하는 걸 확인함.

# Liquidate
KeyCloack이 사용하고 있는 migration tool



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

