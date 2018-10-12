FROM ubuntu:18.04

RUN apt-get update && \
    apt-get install -y apt-utils && \
    apt-get install -y chicken-bin libchicken-dev && \
    apt-get install -y build-essential && \
    apt-get install -y software-properties-common && \
    apt-get install -y curl wget vim unzip git && \
    chicken-install numbers utf8 parley && \
    rm -rf /var/lib/apt/lists/*

ADD csirc /root/.csirc

# (system "bash")
CMD ["csi", "-q"]


