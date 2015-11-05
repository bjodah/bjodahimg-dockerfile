# DO NOT EDIT, This Dockerfile is generated from ./tools/10_generate_Dockerfile.sh
FROM bjodah/bjodahimgbase:v1.0
MAINTAINER Björn Dahlgren <bjodah@DELETEMEgmail.com>
RUN \
    apt-get update && apt-get --quiet --assume-yes install     texlive-bibtex-extra \ 
    texlive-lang-swedish texlive-science texlive-latex-recommended \
    dvipng texlive-fonts-recommended texlive-generic-recommended \
    texlive-latex-extra graphviz dot2tex biber \
    libfreetype6-dev libpng12-dev libjpeg-dev \
    libgmp-dev libmpfr-dev \
    phantomjs imagemagick \
    libopenmpi-dev \
    libatlas-base-dev \
    python-pip python3-pip \
    python-numpy python3-numpy \
    python-matplotlib python3-matplotlib \
    python-mako python3-mako \
    python-mpmath python3-mpmath && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
RUN \
    cd /tmp && \
    wget --quiet http://hera.physchem.kth.se/~repo/bjodahimg/latest/pypi/setuptools-18.4.tar.gz && \
    tar xvzf setuptools-*.tar.gz  && \
    cd setuptools-*  && \
    python2 setup.py install && \
    python3 setup.py install && \
    hash -r  && \
    for FNAME in alabaster-0.7.6.tar.gz apipkg-1.4.tar.gz argh-0.26.1.tar.gz Babel-2.1.1.tar.gz backports_abc-0.4.tar.gz backports.ssl_match_hostname-3.4.0.2.tar.gz blinker-1.4.tar.gz certifi-2015.9.6.2.tar.gz coverage-4.0.1.tar.gz coveralls-1.1.tar.gz Cython-0.23.4.tar.gz decorator-4.0.4.tar.gz docopt-0.6.2.tar.gz docutils-0.12.tar.gz execnet-1.4.1.tar.gz feedgenerator-1.7.tar.gz future-0.15.2.tar.gz ipykernel-4.1.1.tar.gz ipython-4.0.0.tar.gz ipython_genutils-0.1.0.tar.gz ipywidgets-4.1.1.tar.gz Jinja2-2.8.tar.gz jsonschema-2.5.1.tar.gz jupyter-1.0.0.tar.gz jupyter_client-4.1.1.tar.gz jupyter_console-4.0.3.tar.gz jupyter_core-4.0.6.tar.gz MarkupSafe-0.23.tar.gz mistune-0.7.1.tar.gz nbconvert-4.0.0.tar.gz nbformat-4.0.1.tar.gz notebook-4.0.6.tar.gz numpydoc-0.5.tar.gz path.py-8.1.2.tar.gz pelican-3.6.3.tar.gz pep8-1.6.2.tar.gz periodictable-1.4.1.tar.gz pexpect-4.0.1.tar.gz pickleshare-0.5.tar.gz ptyprocess-0.5.tar.gz py-1.4.30.tar.gz pycodeexport-0.1.0.tar.gz pycompilation-0.4.2.tar.gz pyflakes-1.0.0.tar.gz Pygments-2.0.2.tar.gz pyparsing-2.0.4.tar.gz pytest-2.8.2.tar.gz pytest-cache-1.0.tar.gz pytest-cov-2.2.0.tar.gz pytest-flakes-1.0.1.tar.gz pytest-pep8-1.0.6.tar.gz python-dateutil-2.4.2.tar.gz pytz-2015.7.tar.bz2 pyzmq-14.7.0.tar.gz qtconsole-4.1.0.tar.gz quantities-0.10.1.tar.gz requests-2.8.1.tar.gz scipy-0.16.1.tar.gz simplegeneric-0.8.1.zip singledispatch-3.4.0.3.tar.gz six-1.10.0.tar.gz snowballstemmer-1.2.0.tar.gz Sphinx-1.3.1.tar.gz sphinx_rtd_theme-0.1.9.tar.gz sympy-0.7.6.1.tar.gz tornado-4.3b2.tar.gz traitlets-4.0.0.tar.gz Unidecode-0.04.18.tar.gz ; do \
        wget --quiet http://hera.physchem.kth.se/~repo/bjodahimg/latest/pypi/$FNAME -O /tmp/$FNAME; \
    done && \
    for PYPKG in scipy future cython sympy pytest pytest-pep8 pytest-cov pytest-flakes sphinx periodictable pycompilation pycodeexport pelican coveralls numpydoc jupyter argh quantities ; do \
        easy_install-2.7 --always-unzip --allow-hosts=None --find-links file:///tmp/ $PYPKG; \
        easy_install-3.4 --always-unzip --allow-hosts=None --find-links file:///tmp/ $PYPKG; \
    done && \
    for FNAME in {boost-all_1.59.0-1_amd64.deb boost-all-dev_1.59.0-1_amd64.deb boost-build_1.59.0-1_amd64.deb libgsl2_2.0-1_amd64.deb libsundials-serial_2.6.2-1_amd64.deb }; do \
        FILE=$(mktemp); wget "http://hera.physchem.kth.se/~repo/bjodahimg/latest/dpkg/$FNAME" -qO $FILE && sudo dpkg -i $FILE; rm $FILE; \
    done && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
    mkdir -p /root/.config/matplotlib/ && \
    echo "backend: Agg" > /root/.config/matplotlib/matplotlibrc && \
    sed -i 's/TkAgg/Agg/g' /etc/matplotlibrc
RUN \
    #apt-get update && apt-get --quiet --assume-yes install libzmq3-dev && \
    #apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
    easy_install-2.7 /usr/local/lib/python2.7/dist-packages/*-py2.7.egg && \
    easy_install-3.4 /usr/local/lib/python3.4/dist-packages/*-py3.4.egg
