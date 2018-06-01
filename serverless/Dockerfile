FROM node:9-alpine

WORKDIR /app
COPY . .

RUN apk add --no-cache openjdk8

RUN npm install -g npm@latest

RUN npm install -g serverless \
    && npm install serverless-dynamodb-local

RUN serverless dynamodb install 