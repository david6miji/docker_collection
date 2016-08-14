FROM david6miji/gulp-kor:latest

MAINTAINER David You <david6miji@gmail.com>

ENV DEBIAN_FRONTEND noninteractive

# network util
RUN apt-get install -y net-tools

# docker 
WORKDIR /tmp/
RUN	wget -qO- https://get.docker.com/ | sh

# gulp-tool 
ENV PATH $PATH:/gulp-tool/

WORKDIR /work

CMD	bash
