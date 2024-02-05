FROM docker.io/mdehling/ubuntu-dev:2024.02.05

RUN wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/cuda-keyring_1.1-1_all.deb && \
	apt-get -y install ./cuda-keyring_1.1-1_all.deb && \
	rm -f ./cuda-keyring_1.1-1_all.deb
RUN apt-get update

ARG cuda_version='cuda11.8'
ARG cudnn_version='8.9.7.29-1'
RUN apt-get -y install libcudnn8-dev=${cudnn_version}+${cuda_version}
RUN apt-get -y install cuda-toolkit-11-8

ENV PATH=/usr/local/cuda/bin:$PATH
