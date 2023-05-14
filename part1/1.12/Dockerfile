FROM node:16-alpine3.16

EXPOSE 5000

WORKDIR /usr/src/app

RUN apk add --update curl
# RUN apt install -y nodejs

RUN curl -sL https://deb.nodesource.com/setup_16.x



COPY package.json package-lock.json .

RUN npm install

COPY . .

RUN npm run build

RUN npm install -g serve

CMD ["serve", "-s", "-l", "5000", "build"]

