FROM node:latest

WORKDIR /app

COPY ./retryables_tracker .

RUN yarn install

ENTRYPOINT ["yarn"]