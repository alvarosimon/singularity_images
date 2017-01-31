BootStrap: docker
From: tensorflow/tensorflow:latest 
IncludeCmd: yes

%runscript
    exec /usr/bin/python "$@"

%post
    apt-get update && apt-get -y upgrade
    apt-get install vim
    apt-get install git

%test
    # This runs usually less then 30 minutes depending on your host type
    python -m tensorflow.models.image.mnist.convolutional

