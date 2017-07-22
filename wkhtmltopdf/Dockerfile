FROM debian:jessie

MAINTAINER Dietrich Rordorf <dr@ediqo.com>

RUN export DEBIAN_FRONTEND=noninteractive && \
    apt-get update && \
    apt-get -y install apt-utils && \
    apt-get -yq install openssl libssl-dev xorg xvfb fontconfig wget && \
    cd /tmp && \
    wget https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.4/wkhtmltox-0.12.4_linux-generic-amd64.tar.xz && \
    tar -xvf wkhtmltox-0.12.4_linux-generic-amd64.tar.xz && \
    cd wkhtmltox/bin/ && \
    cp * /usr/bin/ && \
    rm -rf /tmp/wkhtmltox

WORKDIR /

CMD ["-h"]
