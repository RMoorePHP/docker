FROM phusion/baseimage:latest

RUN DEBIAN_FRONTEND=noninteractive

RUN locale-gen en_US.UTF-8

ENV LANGUAGE=en_US.UTF-8
ENV LC_ALL=en_US.UTF-8
ENV LC_CTYPE=en_US.UTF-8
ENV LANG=en_US.UTF-8
ENV TERM xterm

RUN apt-get update -y && apt-get install curl

RUN curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -

RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list


RUN apt-get update -y && apt-get install nodejs yarn


CMD yarn && npm run watch