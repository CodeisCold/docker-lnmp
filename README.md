# docker-lnmp
利用docker compose 建立的 lnmp 开发环境

## 目录结构
- `conf`: 配置文件
- `log`: 日志文件
- `app`: 各项目文件目录
- `mysql`: mysql 数据
- `postgres`: postgres 数据

## 部署
- 运行 `docker volume create --name postgres-volume` 用来给 postgres 数据持久化，防止`docker-compose down`后数据消失
- 运行 `docker volume create --name mongodb-volume` 用来给 mongodb 数据持久化，防止`docker-compose down`后数据消失
- 在当前目录下运行 docker-compose up -d

## 使用
- `docker-compose up -d` 创建容器, `-d` 表示后台运行
- `docker-compose down` 销毁容器
- `docker-compose start` 启动容器
- `docker-compose stop` 停止容器
- `docker-compsoe exec namexxx bash` 使用指定容器的shell

## 注意
- 对于挂载的共享目录下的文件，修改后即时生效；对于挂载的单个文件，修改后需要重启容器



