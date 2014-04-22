# DOCKER-VERSION 0.10.0

FROM ubuntu:12.04

RUN echo deb http://archive.ubuntu.com/ubuntu precise universe >> /etc/apt/sources.list
RUN apt-get update -y

#install dependencies
RUN apt-get -y install build-essential libssl-dev wget

#configuration for node
ENV NODE_VERSION 0.10.26
ENV NODE_ARCH x64

#installation node
WORKDIR /tmp
RUN wget http://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$NODE_ARCH.tar.gz
RUN tar xvzf node-v$NODE_VERSION-linux-$NODE_ARCH.tar.gz
RUN rm -rf /opt/nodejs
RUN mv node-v$NODE_VERSION-linux-$NODE_ARCH /opt/nodejs

RUN ln -sf /opt/nodejs/bin/node /usr/bin/node
RUN ln -sf /opt/nodejs/bin/npm /usr/bin/npm

CMD ["node"]
