FROM node:alpine-latest

RUN mkdir /app
WORKDIR /app

COPY package*.json ./

RUN npm install

COPY tsconfig.json ./
COPY public public
COPY src src

CMD ["npm", "run", "start"]