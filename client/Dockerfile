FROM node:14-slim

WORKDIR /usr/src/app

# package.json과 yarn.lock을 WORKDIR에 복사
COPY ./package.json ./yarn.lock ./package-lock.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD [ "npm", "start" ]