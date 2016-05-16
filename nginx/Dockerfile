FROM nginx:stable-alpine
MAINTAINER Alik hochner <alikh@baloota.com>

RUN rm -v /etc/nginx/conf.d/default.conf
ONBUILD COPY build/sixpack.conf /etc/nginx/conf.d/sixpack.conf
ONBUILD COPY certs/* /etc/nginx/certs/
ONBUILD COPY build/htpasswd /etc/nginx/.htpasswd
