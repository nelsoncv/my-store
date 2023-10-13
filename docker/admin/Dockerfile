FROM node:latest

WORKDIR /app/admin

COPY . .

RUN rm -rf node_modules

RUN apt-get update

RUN npm install -g npm@latest

RUN npm install --loglevel=error

RUN npm run build:admin &> /dev/null

CMD [ "medusa-admin", "develop"]