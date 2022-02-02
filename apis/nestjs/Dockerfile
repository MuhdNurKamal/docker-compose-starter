FROM node:16-alpine as builder

ENV NODE_ENV development

WORKDIR /home/node

COPY . /home/node

RUN yarn install --frozen-lockfile \
    && yarn build 

CMD ["yarn", "start:dev"]