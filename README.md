# Docker: node + nginx + PostgreSQL
## Overview
> Dockerを用いて、Node.js + nginx + PostgreSQLのシンプルな環境の構築を行っています。
<br>

## Setup

``` bash
# setup postgresql
$ docker-compose up postgresql

# setup pgadmin
$ docker-compose up pgadmin

# setup app
$ docker-compose up app

# setup web
$ docker-compose up web
```
