# base image
FROM node:alpine

# set working directory
RUN mkdir -p /usr/src/app

COPY package.json .

RUN npm install && npm install --only=dev

ENV NODE_ENV=development

COPY . .

CMD [ "npm", "start" ]