#FROM ubuntu:latest
#LABEL authors="pinyi"
#
#ENTRYPOINT ["top", "-b"]

# 使用官方的 MySQL 映像檔
FROM mysql:8.0

# 設置 MySQL root 用戶的密碼
ENV MYSQL_ROOT_PASSWORD=rootpassword

# 設置初始化時要創建的數據庫名稱
ENV MYSQL_DATABASE=demo_springbootdeploy

# 將 MySQL 配置文件夾掛載到容器內的配置目錄
VOLUME /my/own/datadir:/var/lib/mysql

# 暴露 MySQL 的默認端口 (改 3307)
EXPOSE 3307

# 運行 MySQL 容器時的初始化命令
CMD ["mysqld"]
