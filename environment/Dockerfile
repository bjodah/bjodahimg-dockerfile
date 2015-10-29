# DO NOT EDIT, This Dockerfile is generated from ./tools/10_generate_Dockerfile.sh
FROM bjodah/bjodahimgbase:latest
MAINTAINER Björn Dahlgren <bjodah@DELETEMEgmail.com>
COPY resources /resources
RUN dpkg -i /resources/packages/*.deb && \
    apt-get update && \
    apt-get --quiet --assume-yes install \
    texlive-bibtex-extra \ 
    texlive-lang-swedish texlive-science texlive-latex-recommended \
    dvipng texlive-fonts-recommended texlive-generic-recommended \
    texlive-latex-extra graphviz dot2tex biber \
    libfreetype6-dev libpng12-dev \
    libgmp-dev libmpfr-dev \
    libopenmpi-dev \
    libgsl0-dev \
    python-pip python3-pip \
    python-numpy python3-numpy \
    python-matplotlib python3-matplotlib \
    python-mako python3-mako \
    python-mpmath python3-mpmath && \
    pip install -r /resources/python_packages.txt --find-links file:///resources/pypi_download/ && \
    pip3 install -r /resources/python_packages.txt --find-links file:///resources/pypi_download/ && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
    mkdir -p /root/.config/matplotlib/ && \
    echo "backend: Agg" > /root/.config/matplotlib/matplotlibrc && \
    sed -i 's/TkAgg/Agg/g' /etc/matplotlibrc
