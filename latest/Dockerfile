FROM node:alpine

RUN mkdir /kamino-web-bff

ADD . kamino-web-bff/ 

WORKDIR  kamino-web-bff 

RUN node -v && yarn -v

RUN yarn install

EXPOSE 4000

CMD npm run serve
