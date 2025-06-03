FROM ubuntu:jammy

RUN apt-get update
RUN apt-get install -y python3 build-essential gcc-arm-none-eabi sudo srecord wget

RUN adduser --disabled-password --gecos "" developer && \
  usermod -a -G sudo developer && \
  echo "%sudo ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/nopasswd

ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin

USER developer
WORKDIR /home/developer
