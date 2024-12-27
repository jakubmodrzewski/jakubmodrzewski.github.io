FROM ubuntu:22.04

RUN apt-get update -y && apt-get upgrade -y
RUN apt-get install ruby-full build-essential zlib1g-dev git -y
RUN gem install jekyll bundler

ENV HOME=/home/user
ENV GEM_HOME=/home/user/gems
ENV PATH=/home/user/gems/bin:$PATH
EXPOSE 4000
RUN ruby --version
RUN gem --version