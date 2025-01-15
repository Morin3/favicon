FROM node:18.20.5 as server

WORKDIR /app
COPY ./package.json ./
COPY ./yarn.lock ./
RUN yarn install

COPY . .

RUN yarn build

CMD ["node", "dist/main"]
