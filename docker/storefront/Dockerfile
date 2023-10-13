FROM node:latest

WORKDIR /app/storefront

COPY ./my-medusa-storefront .

RUN rm -rf node_modules

RUN apt-get update

RUN yarn

ENTRYPOINT ["yarn", "dev"]