FROM acrelle/rpi-mqtt-launcher:linux-amd64

LABEL maintainer="anthony@relle.co.uk"

RUN apt-get update && \
 apt-get install -y lirc && \
 rm -rf /var/lib/apt/lists/*

COPY hardware.conf lircd.conf /etc/lirc/
COPY start.sh /app

