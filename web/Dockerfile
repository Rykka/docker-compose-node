FROM node:0.10.38

RUN mkdir /web

WORKDIR /web

RUN npm install nodemon -g
RUN npm install gulp -g
RUN npm install bower -g

ADD package.json package.json
RUN npm install

ADD bower.json bower.json
RUN bower install --allow-root

ADD nodemon.json nodemon.json
ADD gulpfile.js gulpfile.js
ADD gulp gulp
ADD config config
