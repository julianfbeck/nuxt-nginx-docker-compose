FROM node:alpine
RUN apk add --no-cache git
RUN apk add --no-cache openssh
RUN apk add --no-cache yarn
RUN mkdir -p /app
COPY ./app/ /app/
WORKDIR /app
RUN yarn install

# Set environment variables

RUN yarn build
RUN yarn cache clean

EXPOSE 3000

CMD [ "yarn", "start" ]