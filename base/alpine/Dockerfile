FROM alpine:edge

MAINTAINER Matt Hamann <matthew.hamann@gmail.com>

RUN  apk add --update git curl bash \
  && apk del git curl \
  && rm -rf /var/cache/apk/* /usr/local/src/*

CMD []
