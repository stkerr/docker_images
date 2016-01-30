FROM debian:jessie

RUN apt-get -qq update && \
    apt-get -qq -y install \
        avrdude \
        avrdude-doc \
        gcc-avr \
        gdb-avr \
        vim \
        exuberant-ctags \
        git-all \
        python \
        gcc \
        g++ \
        make


RUN git clone https://github.com/stkerr/Config-Files.git &&\
    cd Config-Files && \
    git submodule update --init --recursive && \
    ./deploy.sh -no-terminal-updates

