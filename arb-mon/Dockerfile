FROM buildkite/puppeteer:latest

WORKDIR /app

COPY ./arb-monitoring .

RUN yarn install

ENTRYPOINT ["yarn"]

