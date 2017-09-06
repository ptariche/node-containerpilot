FROM node:8.2

ENV CONTAINERPILOT_VERSION=3.1.3
ENV CONTAINERPILOT_SOURCE=https://github.com/joyent/containerpilot/releases/download/$CONTAINERPILOT_VERSION/containerpilot-$CONTAINERPILOT_VERSION.tar.gz
ENV CONTAINERPILOT=file:///etc/containerpilot.json

# get ContainerPilot release
RUN curl -Lo /tmp/cb.tar.gz $CONTAINERPILOT_SOURCE && \
      tar -xz -f /tmp/cb.tar.gz && \
      mv containerpilot /bin/
