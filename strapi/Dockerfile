FROM node:18.2.0-alpine3.15

COPY ./package.json      /srv/package.json
COPY ./package-lock.json /srv/package-lock.json
COPY ./favicon.ico       /srv/favicon.ico
COPY ./config            /srv/config
COPY ./database          /srv/database
COPY ./public            /srv/public
COPY ./src               /srv/src

WORKDIR /srv
RUN npm install

CMD npm run develop