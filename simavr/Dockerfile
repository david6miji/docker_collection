FROM david6miji/gulp-tool:latest

MAINTAINER David You <david6miji@gmail.com>

ENV DEBIAN_FRONTEND noninteractive

# Install MongoDB.
RUN apt-get install -y gcc-avr
RUN apt-get install -y avr-libc
RUN apt-get install -y libelf-dev
RUN apt-get install -y gtkwave
RUN apt-get install -y build-essential
RUN apt-get install -y freeglut3-dev
RUN apt-get install -y texinfo

WORKDIR /tmp/

RUN git clone git://github.com/buserror-uk/simavr.git

WORKDIR /tmp/simavr
RUN make all
RUN make install 

# Define working directory.
WORKDIR /work

