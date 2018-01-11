FROM node:alpine

ENV GRAPHQL_PORT=4000
ENV REST_API_PORT=3000
ENV NPM_TASK = "start"


RUN mkdir bff
ADD . bff/
WORKDIR bff 
RUN node -v && yarn -v
RUN yarn install

EXPOSE $GRAPHQL_PORT
EXPOSE $REST_API_PORT

CMD npm run $NPM_TASK
