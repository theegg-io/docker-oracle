FROM ubuntu:16.04
MAINTAINER Ludwring Liccien <ludwring.liccien@gmail.com>

ENV DEBIAN_FRONTEND noninteractive 
ENV TERM xterm

# install 
RUN apt-get update -y && \
    apt-get install -y supervisor && \
    apt-get autoclean && apt-get autoremove && \
    rm -rf /var/lib/apt/lists/*

CMD ["/usr/bin/supervisord", "-n"]