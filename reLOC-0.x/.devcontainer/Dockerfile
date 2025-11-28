FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        build-essential \
        python2 \
    && if [ ! -e /usr/local/bin/python ]; then ln -s /usr/bin/python2 /usr/local/bin/python; fi \
    && rm -rf /var/lib/apt/lists/*
