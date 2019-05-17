BootStrap: docker
From: python:3.6.8-slim

%files
    ./requirements.txt /tmp/

%post
    BUILDPKGS="build-essential apt-utils
        python3-dev libhdf5-dev libfreetype6-dev libtool \
        m4 autoconf automake patch bison flex libpng-dev libopenblas-dev \
        tcl-dev tk-dev libxml2-dev zlib1g-dev libffi-dev cmake"
    apt-get update
    apt-get install -y debconf locales && dpkg-reconfigure locales
    apt-get install -y $BUILDPKGS
    ### run time:
    apt-get install -y zlib1g hdf5-tools gfortran libgcc1 libstdc++ musl \
        libopenblas-base tcl tk libxml2 libffi6 less procps

    pip3 install --no-cache-dir --upgrade pip
    pip3 install --no-cache-dir -r /tmp/requirements.txt
    pip install --no-cache-dir ipykernel 

    apt-get remove --purge -y $BUILDPKGS && \
    rm -rf /var/lib/apt/lists/*

