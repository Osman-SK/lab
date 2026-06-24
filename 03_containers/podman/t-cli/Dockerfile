FROM ubuntu:24.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y \
    rtorrent \
    transmission-cli \
    w3m \
    curl \
    wget \
    aria2 \
    nano \
    ca-certificates \
    && rm -rf /var/lib/apt/lists/*

RUN useradd -m -u 1001 torrentuser
USER 1001
WORKDIR /home/torrentuser

CMD ["bash"]
