FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get -y install ssh tmux
RUN apt-get -y install python3 python3-pip python3-venv python3-dev
RUN apt-get -y install software-properties-common

RUN add-apt-repository ppa:neovim-ppa/unstable
RUN apt-get update
RUN apt-get -y install neovim
