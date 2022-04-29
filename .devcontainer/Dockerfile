FROM ubuntu:latest

ARG git_email

RUN apt-get update && DEBIAN_FRONTEND=noninteractive TZ=Etc/UTC apt-get install -y \
    git \
    gcc \
    gdb \
    cmake \
    build-essential

RUN git config --global user.email $git_email
RUN git config --global --add safe.directory '*'

volume /home/

workdir /home/
