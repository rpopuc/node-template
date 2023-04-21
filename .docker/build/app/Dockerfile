ARG NODE_IMAGE_VERSION=alpine3.17
FROM node:${NODE_IMAGE_VERSION}

RUN  apk add bash
COPY entrypoint.sh /
RUN  chmod +x /entrypoint.sh

VOLUME [ "/var/www/" ]
WORKDIR /var/www/

CMD [ "/entrypoint.sh" ]