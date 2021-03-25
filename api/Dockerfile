# Dockerfile that defines the API service.

FROM node:alpine

RUN adduser tracktor -s /bin/sh -D
WORKDIR /home/tracktor/

COPY --chown=node:node ./package.json package.json
COPY --chown=node:node ../yarn.lock yarn.lock

RUN yarn

COPY . .
RUN yarn build

USER tracktor

ENTRYPOINT ["node", "dist/index.js"]