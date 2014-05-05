# DOCKER-VERSION 0.10.0

FROM haklop/nodejs:0.10.28

#install build tools

RUN apt-get -y install fontconfig

RUN npm install -g grunt-cli
RUN npm install -g bower
RUN npm install -g yo
RUN npm install -g less
RUN npm install -g jshint
RUN npm isntall -g mocha
RUN npm install -g phantomjs
RUN npm install -g casperjs

CMD ["node"]
