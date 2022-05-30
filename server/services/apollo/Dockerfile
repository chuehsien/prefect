FROM node:10.23.3
ARG VERSION
ENV SERVER_VERSION=latest

COPY . /apollo

RUN \
    cd /apollo \
    && npm ci && npm run build

WORKDIR /apollo

CMD ["npm", "run", "serve"]
