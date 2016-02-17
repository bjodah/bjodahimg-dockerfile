# DO NOT EDIT, This Dockerfile is generated from ./tools/10_generate_Dockerfile.sh
FROM bjodah/bjodahimgbase:v1.3
MAINTAINER Björn Dahlgren <bjodah@DELETEMEgmail.com>
RUN \
    apt-get update && apt-get --quiet --assume-yes --no-install-recommends install     texlive-generic-recommended texlive-latex-recommended texlive-science texlive-fonts-recommended \
    texlive-latex-extra  texlive-lang-swedish lmodern latex-xcolor texlive-bibtex-extra biber \
    graphviz dot2tex dvipng \
    libfreetype6-dev libpng12-dev libjpeg-dev freeglut3-dev \
    libgmp-dev libmpfr-dev \
    libzmq3-dev libxslt1-dev libxml2-dev \
    phantomjs imagemagick \
    libopenmpi-dev \
    libatlas-base-dev \
    python-matplotlib python3-matplotlib \
    python-mako python3-mako \
    python-mpmath python3-mpmath && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
RUN \
    cd /tmp && \
    for FNAME in boost-all_1.60.0-1_amd64.deb boost-all-dev_1.60.0-1_amd64.deb boost-build_1.60.0-1_amd64.deb libglfw_3.1.2-1_amd64.deb libgsl2_2.1-1_amd64.deb coinor-libipopt1_3.12.4-1_amd64.deb python3-cython_0.23.4-1_amd64.deb python3-scipy_0.17.0-1_amd64.deb python-cython_0.23.4-1_amd64.deb python-scipy_0.17.0-1_amd64.deb libsundials-serial_2.6.2-1_amd64.deb; do \
        wget --no-verbose "http://hera.physchem.kth.se/~repo/bjodahimg/v1.2/dpkg/$FNAME"; \
    done && \
    dpkg -i --force-overwrite boost-all_1.60.0-1_amd64.deb boost-all-dev_1.60.0-1_amd64.deb boost-build_1.60.0-1_amd64.deb libglfw_3.1.2-1_amd64.deb libgsl2_2.1-1_amd64.deb coinor-libipopt1_3.12.4-1_amd64.deb python3-cython_0.23.4-1_amd64.deb python3-scipy_0.17.0-1_amd64.deb python-cython_0.23.4-1_amd64.deb python-scipy_0.17.0-1_amd64.deb libsundials-serial_2.6.2-1_amd64.deb && \
    rm boost-all_1.60.0-1_amd64.deb boost-all-dev_1.60.0-1_amd64.deb boost-build_1.60.0-1_amd64.deb libglfw_3.1.2-1_amd64.deb libgsl2_2.1-1_amd64.deb coinor-libipopt1_3.12.4-1_amd64.deb python3-cython_0.23.4-1_amd64.deb python3-scipy_0.17.0-1_amd64.deb python-cython_0.23.4-1_amd64.deb python-scipy_0.17.0-1_amd64.deb libsundials-serial_2.6.2-1_amd64.deb && \
    cd /tmp && \
    wget --quiet http://hera.physchem.kth.se/~repo/bjodahimg/v1.2/pypi/setuptools-20.1.1.tar.gz && \
    tar xvzf setuptools-*.tar.gz  && \
    cd setuptools-*  && \
    python2 setup.py install && \
    python3 setup.py install && \
    hash -r  && \
    for FNAME in alabaster-0.7.7.tar.gz apipkg-1.4.tar.gz argh-0.26.1.tar.gz Babel-2.2.0.tar.gz backports_abc-0.4.tar.gz backports.ssl_match_hostname-3.5.0.1.tar.gz blinker-1.4.tar.gz bokeh-0.11.1.tar.gz bottle-0.12.9.tar.gz cclib-1.3.tar.gz certifi-2015.11.20.1.tar.gz CherryPy-5.0.1.tar.gz cloudpickle-0.1.1.tar.gz coverage-4.0.3.tar.gz coveralls-1.1.tar.gz decorator-4.0.6.tar.gz docopt-0.6.2.tar.gz docutils-0.12.tar.gz doit-0.29.0.tar.gz execnet-1.4.1.tar.gz fastcache-1.0.2.tar.gz Flask-0.10.1.tar.gz future-0.15.2.tar.gz futures-3.0.4.tar.gz ghp-import2-1.0.1.tar.gz glfw-1.1.2.tar.gz gr-0.17.3.tar.gz grip-4.1.0.zip husl-4.0.3.tar.gz ipykernel-4.2.2.tar.gz ipython-4.1.1.tar.gz ipython_genutils-0.1.0.tar.gz ipywidgets-4.1.1.tar.gz itsdangerous-0.24.tar.gz Jinja2-2.8.tar.gz joblib-0.9.4.tar.gz jsonschema-2.5.1.tar.gz jupyter-1.0.0.tar.gz jupyter_client-4.1.1.tar.gz jupyter_console-4.1.0.tar.gz jupyter_core-4.0.6.tar.gz Logbook-0.12.5.tar.gz lxml-3.5.0.tar.gz Mako-1.0.3.tar.gz Markdown-2.6.5.tar.gz MarkupSafe-0.23.tar.gz micawber-0.3.3.tar.gz mistune-0.7.1.tar.gz mogli-0.2.3.tar.gz mpld3-0.2.tar.gz natsort-4.0.4.tar.gz nbconvert-4.1.0.tar.gz nbformat-4.0.1.tar.gz nikola-7.7.5.tar.gz notebook-4.1.0.tar.gz numpy-1.10.4.tar.gz numpydoc-0.6.0.tar.gz ordered-set-2.0.0.tar.gz pandas-0.17.1.tar.gz path-and-address-1.0.0.zip path.py-8.1.2.tar.gz pathtools-0.1.2.tar.gz patsy-0.4.1.zip pep8-1.7.0.tar.gz periodictable-1.4.1.tar.gz pexpect-4.0.1.tar.gz phpserialize-1.3.tar.gz pickleshare-0.6.tar.gz Pillow-3.1.1.tar.gz pip-8.0.2.tar.gz ptyprocess-0.5.1.tar.gz py-1.4.31.tar.gz pycodeexport-0.1.0.tar.gz pycompilation-0.4.2.tar.gz pyflakes-1.0.0.tar.gz pygal-2.1.1.tar.gz Pygments-2.1.tar.gz pyinotify-0.9.6.tar.gz PyLaTeX-1.0.0.tar.gz PyOpenGL-3.1.0.tar.gz pyparsing-2.1.0.tar.gz Pyphen-0.9.4.tar.gz PyRSS2Gen-1.1.tar.gz pytest-2.8.7.tar.gz pytest-cache-1.0.tar.gz pytest-cov-2.2.1.tar.gz pytest-flakes-1.0.1.tar.gz pytest-pep8-1.0.6.tar.gz python-dateutil-2.4.2.tar.gz pytz-2015.7.tar.bz2 PyYAML-3.11.tar.gz pyzmq-15.2.0.tar.gz qtconsole-4.1.1.tar.gz quantities-0.11.1.zip requests-2.9.1.tar.gz setuptools_scm-1.10.1.tar.bz2 simplegeneric-0.8.1.zip singledispatch-3.4.0.3.tar.gz six-1.10.0.tar.gz smartypants-1.8.6.tar.gz snowballstemmer-1.2.1.tar.gz Sphinx-1.3.5.tar.gz sphinx_rtd_theme-0.1.9.tar.gz SQLAlchemy-1.0.11.tar.gz statsmodels-0.6.1.tar.gz stdeb-0.8.5.tar.gz sympy-0.7.6.1.tar.gz terminado-0.6.tar.gz toolz-0.7.4.tar.gz tornado-4.3.tar.gz traitlets-4.1.0.tar.gz typogrify-2.0.7.tar.gz Unidecode-0.04.19.tar.gz vcversioner-2.14.0.0.tar.gz watchdog-0.8.3.tar.gz webassets-0.11.1.tar.gz Werkzeug-0.11.3.tar.gz ws4py-0.3.4.tar.gz Yapsy-1.11.223.tar.gz ; do \
        wget --quiet http://hera.physchem.kth.se/~repo/bjodahimg/v1.2/pypi/$FNAME -O /tmp/$FNAME; \
    done && \
    for PYPKG in future sympy pytest pytest-pep8 pytest-cov pytest-flakes sphinx periodictable pycompilation pycodeexport coveralls numpydoc jupyter argh quantities fastcache bottle sqlalchemy bokeh mogli pylatex joblib cclib toolz grip statsmodels mpld3 pip stdeb ; do \
        easy_install-2.7 --always-unzip --allow-hosts=None --find-links file:///tmp/ $PYPKG; \
        easy_install-3.4 --always-unzip --allow-hosts=None --find-links file:///tmp/ $PYPKG; \
    done && \
    for PYPKG in CherryPy Nikola[extras] ; do \
        easy_install-3.4 --always-unzip --allow-hosts=None --find-links file:///tmp/ $PYPKG; \
    done && \
    easy_install-2.7 /usr/local/lib/python2.7/dist-packages/*-py2.7.egg && \
    easy_install-3.4 /usr/local/lib/python3.4/dist-packages/*-py3.4.egg && \
    ln -s /usr/local/share/pyphen /usr/share/pyphen && \
    ipython2 kernel install && \
    ipython3 kernel install && \
    mkdir -p /root/.config/matplotlib/ && \
    echo "backend: Agg" > /root/.config/matplotlib/matplotlibrc && \
    sed -i 's/TkAgg/Agg/g' /etc/matplotlibrc && \
    cd /tmp && \
    for FNAME in miniconda2.sh; do \
        wget --no-verbose "http://hera.physchem.kth.se/~repo/bjodahimg/v1.2/blobs/$FNAME"; \
    done && \
    bash miniconda2.sh -b -p /opt/miniconda2 && \
    rm miniconda2.sh && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# RUN \
#     apt-get update && apt-get --quiet --assume-yes --no-install-recommends install MISSING_PACKAGE
