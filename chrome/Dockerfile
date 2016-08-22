# 이것은 미완성이다. 

FROM david6miji/gulp-tool:latest

MAINTAINER David You <david6miji@gmail.com>

ENV DEBIAN_FRONTEND noninteractive

# install librury and tool
RUN apt-get install -y curl
RUN apt-get install -y libgl1-mesa-dri
RUN apt-get install -y libgl1-mesa-glx
RUN apt-get install -y libpulse0
RUN apt-get install -y libv4l-0

# install chrome

RUN curl -sSL https://dl.google.com/linux/linux_signing_key.pub | apt-key add - \
	&& echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" > /etc/apt/sources.list.d/google.list \
	&& apt-get update 

# install hangul font and input method	
RUN apt-get install -y google-chrome-stable
RUN apt-get install -y ttf-unfonts-core
# RUN apt-get install -y nabi
# RUN apt-get update 

# Define working directory.
WORKDIR /work

