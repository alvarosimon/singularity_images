BootStrap: docker
From: centos:latest


%runscript
    echo "This is what happens when you run the container..."


%post
    export EASYBUILD_VERSION="3.0.2"
    yum -y install gcc
    yum -y install make
    yum -y install openssl-devel
    yum -y install libibverbs-devel
    yum -y install tar bzip2 gzip unzip
    yum -y install which
    yum -y install epel-release
    yum -y install python-pip
    yum -y install Lmod
    yum -y install python-setuptools
    yum -y install git
    yum -y install vim
    pip install easybuild==$EASYBUILD_VERSION

