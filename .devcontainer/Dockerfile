FROM ubuntu:latest

RUN apt-get update && DEBIAN_FRONTEND=noninteractive TZ=Etc/UTC apt-get install -y \
    git \
    gcc \
    gdb \
    build-essential

RUN git config --global user.email og.ginger@gmail.com

volume /home/

workdir /home/
