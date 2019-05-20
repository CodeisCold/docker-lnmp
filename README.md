# docker-lnmp
利用docker compose 建立的 lnmp 开发环境

## 目录结构
- `conf`: 配置文件
- `log`: 日志文件
- `app`: 各项目文件目录
- `mysql`: mysql 数据
- `postgres`: postgres 数据

## 使用
- 在当前目录下运行 docker-compose up

## 使用注意
1. 先运行 `docker volume create --name postgres-volume` 用来给 postgres 数据持久化，防止`docker-compose down`后数据消失

