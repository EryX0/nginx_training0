FROM node:18.17.1-alpine3.18
COPY ./package.json ./yarn.lock ./craco.config.js /app/
WORKDIR /app/
RUN yarn install --frozen-lockfile
COPY . /app/
CMD ["sh", "-c", "NODE_OPTIONS=--openssl-legacy-provider yarn start"]
EXPOSE 3000