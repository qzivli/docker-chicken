FROM debian:stretch

COPY sources.list /etc/apt/sources.list

RUN apt-get update && \
    apt-get install -y chicken-bin libchicken-dev && \
    apt-get install -y build-essential && \
    chicken-install r7rs numbers utf8 parley && \
    rm -rf /var/lib/apt/lists/*

ADD csirc /root/.csirc

CMD ["csi", "-q"]

