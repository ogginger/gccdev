FROM ubuntu:latest

ARG git_email

RUN apt-get update && DEBIAN_FRONTEND=noninteractive TZ=Etc/UTC apt-get install -y \
    git \
    gcc \
    gdb \
    cmake \
    build-essential \
    curl \
    zip \
    unzip \
    pkg-config

RUN git config --global user.email $git_email && \
    git config --global --add safe.directory '*'

RUN git clone https://github.com/Microsoft/vcpkg.git /opt/vcpkg && \
    mkdir /root/.vcpkg && \
    /opt/vcpkg/bootstrap-vcpkg.sh -disableMetrics && \
    /opt/vcpkg/vcpkg integrate install
    
ENV PATH "/opt/vcpkg:$PATH"

