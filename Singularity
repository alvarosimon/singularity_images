BootStrap: yum
OSVersion: 7.2.1511
MirrorURL: http://mirror.centos.org/centos-7/%{OSVERSION}/os/$basearch/
Include: yum

# If you want the updates (available at the bootstrap date) to be installed
# inside the container during the bootstrap instead of the General Availability
# point release (7.x) then uncomment the following line
#UpdateURL: http://mirror.centos.org/centos-%{OSVERSION}/%{OSVERSION}/updates/$basearch/


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
    pip install easybuild==$EASYBUILD_VERSION

