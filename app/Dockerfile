# syntax=docker/dockerfile:1
# FROM node:12-alpine
# RUN apk add --no-cache python2 g++ make
# WORKDIR /app
# COPY . .
# RUN yarn install --production
# CMD ["node", "src/index.js"]



 # syntax=docker/dockerfile:1
 # cached version
 FROM node:12-alpine
 RUN apk add --no-cache python2 g++ make
 WORKDIR /app
 COPY package.json yarn.lock ./
 RUN yarn install --production
 COPY . .
 CMD ["node", "src/index.js"]
 EXPOSE 3000