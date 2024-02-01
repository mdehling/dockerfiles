FROM docker.io/library/docker:25.0-dind

RUN apk add openrc docker
RUN rc-update add docker

RUN apk add openssh
RUN rc-update add sshd

RUN apk add git tmux neovim
