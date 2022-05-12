FROM node:10.24.0
ARG VERSION
ENV SERVER_VERSION=latest

COPY . /apollo

RUN \
    cd /apollo \
    && npm ci && npm run build

WORKDIR /apollo

CMD ["npm", "run", "serve"]
