ARG CUDA_FULL_VERSION
ARG CUDNN_MAJOR_VERSION
ARG UBUNTU_VERSION

FROM nvidia/cuda:${CUDA_FULL_VERSION}-cudnn${CUDNN_MAJOR_VERSION}-runtime-ubuntu${UBUNTU_VERSION}

LABEL maintainer="Tinson Lai"
LABEL org.opencontainers.image.authors="Tinson Lai"
LABEL org.opencontainers.image.vendor="Human Factor Team, Institute of Intelligent Manufacturing, Guangdong Academy of Sciences"
LABEL org.opencontainers.image.base.name="nvidia/cuda"

ARG DEBIAN_FRONTEND=noninteractive

COPY sources.list /etc/apt/sources.list
COPY ubuntu.list /etc/apt/sources.list.d/ubuntu.list
RUN apt-get update
RUN apt-get install -y gcc

ADD https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh /tmp/miniconda.sh
COPY .condarc /root/.condarc
RUN /bin/bash /tmp/miniconda.sh -b -p /opt/conda
RUN /opt/conda/bin/conda install -y --update-all python pip

RUN rm -f /tmp/miniconda.sh
RUN rm -rf /var/lib/apt/lists
RUN /opt/conda/bin/conda clean -ay
