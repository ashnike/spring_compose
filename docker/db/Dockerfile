FROM mysql:latest
LABEL Project="DockerCompo"
LABEL Author="Ashnike"

ENV MYSQL_ROOT_PASSWORD="ashpi123"
ENV MYSQL_DATABASE="accounts"
ENV MYSQL_USER="admin"
ENV MYSQL_PASSWORD="admin123"
ADD  db_backup.sql docker-entrypoint-initdb.d/db_backup.sql
