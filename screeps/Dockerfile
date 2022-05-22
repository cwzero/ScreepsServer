FROM node:10
RUN apt-get update && apt-get install -y build-essential

VOLUME /world
WORKDIR /world

RUN npm config set user 0
RUN npm config set unsafe-perm true

RUN npm install -g node-gyp@latest

RUN npm install screeps
RUN npx screeps init
CMD npx screeps start --steam_api_key 54F1DF71F6C44D1AC2A1B3E32E1FC09E
