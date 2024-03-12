FROM nginx:1.25.4-alpine3.18
LABEL Project="DockerCompo"
LABEL Author="Ashnike"

RUN rm -rf /etc/nginx/conf.d/default.conf
COPY nginxjapp.conf /etc/nginx/conf.d/nginxjapp.conf