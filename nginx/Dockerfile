FROM nginx:1.18.0
MAINTAINER who "lianyan598@gmail.com"

ENV TZ "Asia/Shanghai"
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

COPY nginx.conf /etc/nginx/nginx.conf

RUN mkdir -p /opt/log \
    && mkdir -p /opt/www \
    && bash -c 'chmod 777 -R /opt'