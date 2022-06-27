FROM ghcr.io/giim-hf-lab/hailab/base:ubuntu20.04-cuda11.2.2-cudnn8

LABEL maintainer="Tinson Lai"
LABEL org.opencontainers.image.authors="Tinson Lai"
LABEL org.opencontainers.image.vendor="Human Factor Team, Institute of Intelligent Manufacturing, Guangdong Academy of Sciences"
LABEL org.opencontainers.image.base.name="nvidia/cuda"

RUN /opt/conda/bin/python -m pip install -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/stable.html paddlepaddle-gpu
