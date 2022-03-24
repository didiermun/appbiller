FROM node:14-alpine as builder
WORKDIR /usr/app
COPY ./package.json /usr/app
RUN yarn install 
COPY ./ /usr/app
RUN yarn build
EXPOSE 4000

CMD ["yarn","start"]