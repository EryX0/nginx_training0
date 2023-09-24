FROM node:13.8-alpine3.11 AS builder
COPY ./package.json ./yarn.lock ./tsconfig.json ./tslint.json /app/
WORKDIR /app/
RUN yarn install --frozen-lockfile
COPY . /app/
EXPOSE 3000
CMD ["yarn","start"]