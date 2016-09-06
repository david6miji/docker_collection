FROM david6miji/gulp-tool:latest

MAINTAINER David You <david6miji@gmail.com>

RUN apt-get install -y build-essential
RUN apt-get install -y g++-multilib libc6-dev-i386
RUN apt-get install -y u-boot-tools
RUN apt-get install -y libgmp3-dev libmpfr4 libmpfr-dev

RUN apt-get install -y dkms
RUN apt-get install -y vim

RUN apt-get install -y bc
RUN apt-get install -y unrar-free
RUN apt-get install -y bison
RUN apt-get install -y flex
RUN apt-get install -y minicom

RUN apt-get install -y lib32z1 lib32z1-dev
RUN apt-get install -y liblzo2-2 liblzo2-dev

RUN cp -a /usr/lib/x86_64-linux-gnu/libmpfr* /usr/lib
RUN cp -a /usr/lib/x86_64-linux-gnu/libgmp* /usr/lib

RUN apt-get install -y usbutils libusb-1.0-0-dev libusb-dev
RUN apt-get install -y lzop
RUN apt-get install -y unzip

ADD gcc-linaro-arm-linux-gnueabihf-4.9-2014.09_linux.tgz /opt/
ENV PATH $PATH::/opt/gcc-linaro-arm-linux-gnueabihf-4.9-2014.09_linux/bin/

# Define working directory.
WORKDIR /work
