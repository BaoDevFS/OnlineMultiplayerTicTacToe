FROM node:latest

RUN mkdir -p /usr/src/node-app && chown -R node:node /usr/src/node-app

WORKDIR /usr/src/node-app

COPY package.json /usr/src/node-app
USER node

RUN npm install

COPY --chown=node:node . /usr/src/node-app

EXPOSE 3000







