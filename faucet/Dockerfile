FROM node:latest

WORKDIR /app

RUN apt install git

RUN git clone https://github.com/OffchainLabs/arbtoken_twitter_faucet.git

WORKDIR /app/arbtoken_twitter_faucet

RUN git checkout nitro-faucet

RUN yarn install

ENTRYPOINT ["yarn"]
