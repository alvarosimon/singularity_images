BootStrap: docker
From: tensorflow/tensorflow:latest 
IncludeCmd: yes

%runscript
    exec /usr/bin/python "$@"

%post
    apt-get update && apt-get -y upgrade
    apt-get install -y vim
    apt-get install -y git

