FROM debian:bullseye

RUN apt-get update && \
    apt-get install -y git gcc g++ make cmake vim iproute2 && \
    git clone https://github.com/mz-automation/libiec61850.git && \
    cd libiec61850 && cmake . &&  make -j $(nproc) && make install
