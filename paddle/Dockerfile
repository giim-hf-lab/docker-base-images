FROM ghcr.io/giim-hf-lab/hailab/base:ubuntu20.04-cuda11.2.2-cudnn8-cn

LABEL maintainer="Tinson Lai"
LABEL org.opencontainers.image.authors="Tinson Lai"
LABEL org.opencontainers.image.vendor="Human Factor Team, Institute of Intelligent Manufacturing, Guangdong Academy of Sciences"
LABEL org.opencontainers.image.base.name="nvidia/cuda"

RUN /opt/conda/bin/conda install --yes --update-all -c Paddle paddlepaddle-gpu cudatoolkit=11.2 numpy
RUN /opt/conda/bin/conda clean -ay
