FROM ghcr.io/giim-hf-lab/hailab/base:ubuntu20.04-cuda11.5.2-cudnn8

LABEL maintainer="Tinson Lai"
LABEL org.opencontainers.image.authors="Tinson Lai"
LABEL org.opencontainers.image.vendor="Human Factor Team, Institute of Intelligent Manufacturing, Guangdong Academy of Sciences"
LABEL org.opencontainers.image.base.name="nvidia/cuda"

RUN /opt/conda/bin/python -m pip install --extra-index-url https://download.pytorch.org/whl/cu115 torch torchvision torchaudio
