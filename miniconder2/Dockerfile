FROM phusion/baseimage:0.9.18

# System packages
RUN apt-get update && \
    apt-get install -y wget git

RUN wget http://repo.continuum.io/miniconda/Miniconda2-3.19.0-Linux-x86_64.sh  -O miniconda.sh && \
    bash miniconda.sh -b -p /root/miniconda && \
    rm /miniconda.sh && \
    /root/miniconda/bin/conda config --set always_yes True --set changeps1 True && \
    /root/miniconda/bin/conda update -q conda && \
    /root/miniconda/bin/conda info -a

ENV PATH="/root/miniconda/bin:$PATH"
