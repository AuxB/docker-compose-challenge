FROM node:alpine

ENV PATH /app/node_modules/.bin:$PATH

RUN mkdir /app
WORKDIR /app
COPY package*.json ./
COPY yarn.lock ./
COPY public public
COPY src src
RUN npm i
CMD npm start
