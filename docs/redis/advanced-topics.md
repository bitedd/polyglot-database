---
layout: default
title: Advanced Topics
nav_order: 3
parent: Redis
---
 
# Lock

### classical lock mechanism
* [SETNX (deprecated)](https://redis.io/docs/latest/commands/setnx/#design-pattern-locking-with-codesetnxcode)
  + look the part of "Handling deadlocks"

This lock mechanism may not be reliable in case of Redis master failure.

### Distributed Locks with Redis
* [Redlock](https://redis.io/docs/latest/develop/use/patterns/distributed-locks/)
  + This lock mechanism provide more safe way of locking in distrubuted environment.

