FROM ghcr.io/giim-hf-lab/hailab/base:ubuntu20.04-cuda11.5.2-cudnn8-cn

LABEL org.opencontainers.image.source="https://github.com/giim-hf-lab/docker-base-images"

RUN /opt/conda/bin/conda install --yes --update-all -c pytorch pytorch torchvision torchaudio cudatoolkit=11.5 numpy
RUN /opt/conda/bin/conda clean -ay
