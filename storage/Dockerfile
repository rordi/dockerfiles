FROM debian:jessie

MAINTAINER Dietrich Rordorf <dr@ediqo.com>

VOLUME /data

RUN groupadd -g 1000 storage && useradd -u 1000 -g storage storage

USER root

CMD ["sh", "-c", "tail -f /dev/null"]
