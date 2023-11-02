FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get upgrade -y && apt-get -y clean

RUN apt-get -y install --no-install-recommends nvidia-cuda-toolkit && apt-get -y clean
RUN apt-get -y install --no-install-recommends nvidia-cudnn && apt-get -y clean
ENV XLA_FLAGS=--xla_gpu_cuda_data_dir=/usr/lib/cuda

RUN apt-get -y install python3 python3-pip python3-venv python3-dev
RUN apt-get -y install ssh tmux neovim
