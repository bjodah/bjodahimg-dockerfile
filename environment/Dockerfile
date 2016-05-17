# DO NOT EDIT, This Dockerfile is generated from ./tools/10_generate_Dockerfile.sh
FROM bjodah/bjodahimgbase:v1.3
MAINTAINER Björn Dahlgren <bjodah@DELETEMEgmail.com>
RUN \
    apt-get update && apt-get --quiet --assume-yes --no-install-recommends install     texlive-generic-recommended texlive-latex-recommended texlive-science texlive-fonts-recommended \
    texlive-latex-extra  texlive-lang-swedish lmodern latex-xcolor texlive-bibtex-extra biber \
    graphviz dot2tex dvipng \
    freeglut3-dev \
    expect-dev xutils-dev \
    phantomjs imagemagick \
    python-matplotlib python3-matplotlib \
    python-mako python3-mako \
    python-mpmath python3-mpmath \
    octave \
    libxrender1 fonts-dejavu pandoc \
    python-rdkit librdkit1 rdkit-data && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
RUN \
    cd /tmp && \
    for FNAME in boost-all_1.61.0-1_amd64.deb boost-all-dev_1.61.0-1_amd64.deb boost-build_1.61.0-1_amd64.deb libglfw_3.1.2-1_amd64.deb libgsl2_2.1-1_amd64.deb coinor-libipopt1_3.12.4-1_amd64.deb python3-cython_0.23.4-1_amd64.deb python3-scipy_0.17.0-1_amd64.deb python-cython_0.23.4-1_amd64.deb python-scipy_0.17.0-1_amd64.deb libsundials-serial_2.6.2-1_amd64.deb ; do \
        wget --no-verbose "http://hera.physchem.kth.se/~repo/bjodahimg/latest/dpkg/$FNAME"; \
    done && \
    dpkg -i --force-overwrite boost-all_1.61.0-1_amd64.deb boost-all-dev_1.61.0-1_amd64.deb boost-build_1.61.0-1_amd64.deb libglfw_3.1.2-1_amd64.deb libgsl2_2.1-1_amd64.deb coinor-libipopt1_3.12.4-1_amd64.deb python3-cython_0.23.4-1_amd64.deb python3-scipy_0.17.0-1_amd64.deb python-cython_0.23.4-1_amd64.deb python-scipy_0.17.0-1_amd64.deb libsundials-serial_2.6.2-1_amd64.deb  && \
    rm boost-all_1.61.0-1_amd64.deb boost-all-dev_1.61.0-1_amd64.deb boost-build_1.61.0-1_amd64.deb libglfw_3.1.2-1_amd64.deb libgsl2_2.1-1_amd64.deb coinor-libipopt1_3.12.4-1_amd64.deb python3-cython_0.23.4-1_amd64.deb python3-scipy_0.17.0-1_amd64.deb python-cython_0.23.4-1_amd64.deb python-scipy_0.17.0-1_amd64.deb libsundials-serial_2.6.2-1_amd64.deb && \
    cd /tmp && \
    wget --quiet http://hera.physchem.kth.se/~repo/bjodahimg/latest/pypi/setuptools-21.0.0.tar.gz && \
    tar xvzf setuptools-*.tar.gz  && \
    cd setuptools-*  && \
    python2 setup.py install && \
    python3 setup.py install && \
    cd - && \
    wget --quiet http://hera.physchem.kth.se/~repo/bjodahimg/latest/pypi/pip-8.1.2.tar.gz && \
    tar xvzf pip-*.tar.gz  && \
    cd pip-*  && \
    python2 setup.py install && \
    python3 setup.py install && \
    cd - && \
    hash -r  && \
    for FNAME in alabaster-0.7.8-py2.py3-none-any.whl apipkg-1.4-py2.py3-none-any.whl argh-0.26.2-py2.py3-none-any.whl ase-3.11.0.tar.gz Babel-2.3.4-py2.py3-none-any.whl backports_abc-0.4-py2.py3-none-any.whl backports.shutil_get_terminal_size-1.0.0-py2.py3-none-any.whl backports.ssl_match_hostname-3.5.0.1.tar.gz blinker-1.4.tar.gz bokeh-0.11.1.tar.gz bottle-0.12.9.tar.gz cclib-1.4.tar.gz certifi-2016.2.28-py2.py3-none-any.whl CherryPy-5.4.0-py3-none-any.whl cloudpickle-0.2.1-py2.py3-none-any.whl configparser-3.3.0r2.tar.gz coverage-4.0.3.tar.gz coveralls-1.1-py2.py3-none-any.whl cycler-0.10.0-py2.py3-none-any.whl decorator-4.0.9-py2.py3-none-any.whl docopt-0.6.2.tar.gz docutils-0.12-py3-none-any.whl docutils-0.12.tar.gz doit-0.29.0.tar.gz entrypoints-0.2.1-py2.py3-none-any.whl execnet-1.4.1-py2.py3-none-any.whl fastcache-1.0.2.tar.gz Flask-0.10.1.tar.gz functools32-3.2.3-2.zip future-0.15.2.tar.gz futures-3.0.5-py2-none-any.whl ghp_import2-1.0.1-py2.py3-none-any.whl glfw-1.1.3.tar.gz gr-0.18.0.tar.gz grip-4.2.0.zip holoviews-1.5.0.zip husl-4.0.3.tar.gz imagesize-0.7.1-py2.py3-none-any.whl ipykernel-4.3.1-py2.py3-none-any.whl ipython-4.2.0-py2-none-any.whl ipython-4.2.0-py3-none-any.whl ipython_genutils-0.1.0-py2.py3-none-any.whl ipywidgets-5.1.3-py2.py3-none-any.whl itsdangerous-0.24.tar.gz Jinja2-2.8-py2.py3-none-any.whl joblib-0.9.4-py2.py3-none-any.whl jsonschema-2.5.1-py2.py3-none-any.whl jupyter-1.0.0-py2.py3-none-any.whl jupyter_client-4.2.2-py2.py3-none-any.whl jupyter_console-4.1.1-py2.py3-none-any.whl jupyter_core-4.1.0-py2.py3-none-any.whl lancet-ioam-0.9.0.tar.gz Logbook-0.12.5.tar.gz lxml-3.6.0.tar.gz Mako-1.0.4.tar.gz Markdown-2.6.6.zip MarkupSafe-0.23.tar.gz matplotlib-1.5.1.tar.gz micawber-0.3.3.tar.gz mistune-0.7.2-py2.py3-none-any.whl mogli-0.2.3.tar.gz mpld3-0.2.tar.gz mpmath-0.19.tar.gz natsort-5.0.0-py2.py3-none-any.whl nbconvert-4.2.0-py2.py3-none-any.whl nbformat-4.0.1-py2.py3-none-any.whl Nikola-7.7.8-py2.py3-none-any.whl notebook-4.2.0-py2.py3-none-any.whl numpy-1.11.0.tar.gz numpydoc-0.6.0.tar.gz ordered-set-2.0.1.tar.gz pandas-0.18.1.tar.gz param-1.3.2.tar.gz path-and-address-1.1.0.zip pathlib2-2.1.0-py2.py3-none-any.whl pathtools-0.1.2.tar.gz patsy-0.4.1-py2.py3-none-any.whl pep8-1.7.0-py2.py3-none-any.whl periodictable-1.4.1.tar.gz pexpect-4.0.1.tar.gz phpserialize-1.3.tar.gz pickleshare-0.7.2-py2.py3-none-any.whl Pillow-3.2.0.zip ptyprocess-0.5.1-py2.py3-none-any.whl py-1.4.31-py2.py3-none-any.whl pycodeexport-0.1.0.tar.gz pycompilation-0.4.2.tar.gz pyflakes-1.2.3-py2.py3-none-any.whl pygal-2.2.2-py2.py3-none-any.whl Pygments-2.1.3-py2.py3-none-any.whl pyinotify-0.9.6.tar.gz PyLaTeX-1.0.0.tar.gz PyOpenGL-3.1.0.tar.gz pyparsing-2.1.4-py2.py3-none-any.whl Pyphen-0.9.4-py2.py3-none-any.whl PyRSS2Gen-1.1.tar.gz pytest-2.9.1-py2.py3-none-any.whl pytest-cache-1.0.tar.gz pytest_cov-2.2.1-py2.py3-none-any.whl pytest-flakes-1.0.1.tar.gz pytest-pep8-1.0.6.tar.gz python_dateutil-2.5.3-py2.py3-none-any.whl pytz-2016.4-py2.py3-none-any.whl PyYAML-3.11.zip pyzmq-15.2.0.zip qtconsole-4.2.1-py2.py3-none-any.whl quantities-0.11.1.zip requests-2.10.0-py2.py3-none-any.whl simplegeneric-0.8.1.zip singledispatch-3.4.0.3-py2.py3-none-any.whl six-1.10.0-py2.py3-none-any.whl smartypants-1.8.6-py2.py3-none-any.whl snowballstemmer-1.2.1-py2.py3-none-any.whl Sphinx-1.4.1-py2.py3-none-any.whl SQLAlchemy-1.0.12.tar.gz statsmodels-0.6.1.tar.gz stdeb-0.8.5.tar.gz sympy-1.0.tar.gz terminado-0.6.tar.gz toolz-0.7.4.tar.gz tornado-4.3.tar.gz traitlets-4.2.1-py2.py3-none-any.whl typogrify-2.0.7.tar.gz Unidecode-0.04.19.tar.gz virtualenv-15.0.1-py2.py3-none-any.whl watchdog-0.8.3.tar.gz webassets-0.11.1.tar.gz Werkzeug-0.11.9-py2.py3-none-any.whl widgetsnbextension-1.2.2-py2.py3-none-any.whl ws4py-0.3.4.tar.gz xarray-0.7.2-py2.py3-none-any.whl Yapsy-1.11.223.tar.gz ; do \
        wget --quiet http://hera.physchem.kth.se/~repo/bjodahimg/latest/pypi/$FNAME -O /tmp/$FNAME; \
    done && \
    for PYPKG in future sympy pytest pytest-pep8 pytest-cov pytest-flakes sphinx periodictable pycompilation pycodeexport coveralls numpydoc jupyter argh quantities fastcache bottle sqlalchemy bokeh mogli pylatex joblib cclib toolz grip statsmodels mpld3 pip stdeb param holoviews[recommended] ase virtualenv xarray ; do \
        python2 -m pip install --no-index --find-links file:///tmp/ $PYPKG; \
        python3 -m pip install --no-index --find-links file:///tmp/ $PYPKG; \
    done && \
    for PYPKG in CherryPy Nikola[extras] ; do \
        python3 -m pip install --no-index --find-links file:///tmp/ $PYPKG; \
    done && \
    ln -s /usr/local/share/pyphen /usr/share/pyphen && \
    ipython2 kernel install && \
    ipython3 kernel install && \
    mkdir -p /root/.config/matplotlib/ && \
    echo "backend: Agg" > /root/.config/matplotlib/matplotlibrc && \
    sed -i 's/TkAgg/Agg/g' /etc/matplotlibrc && \
    cd /tmp && \
    for FNAME in miniconda2.sh; do \
        wget --no-verbose "http://hera.physchem.kth.se/~repo/bjodahimg/latest/blobs/$FNAME"; \
    done && \
    bash miniconda2.sh -b -p /opt/miniconda2 && \
    rm miniconda2.sh && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# RUN \
#     apt-get update && apt-get --quiet --assume-yes --no-install-recommends install MISSING_PACKAGE
