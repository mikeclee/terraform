FROM ubuntu:14.04

MAINTAINER Mike Lee <mike.c.lee@disney.com>

RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
    git

RUN gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
RUN curl -L https://get.rvm.io | bash -s stable --ruby
RUN echo "\nsource /usr/local/rvm/scripts/rvm" >> /root/.bashrc
RUN /bin/bash -l -c "gem install jekyll"

EXPOSE 4000
