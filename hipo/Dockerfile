FROM david6miji/simavr:latest

MAINTAINER David You <david6miji@gmail.com>

ENV DEBIAN_FRONTEND noninteractive

# Install arduino core package
WORKDIR /tmp/
RUN apt-get install -y arduino-core

# Define working directory.
WORKDIR /work
