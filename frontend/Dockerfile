# base image
FROM node:12.2.0-alpine

# set working directory
WORKDIR /app

# git is a dependency of installing npm expo
#TODO: split this into build/multistage image
RUN apk update && apk upgrade && \
    apk add --no-cache bash git openssh

# install and cache app dependencies
COPY package.json /app/package.json
RUN npm install

# start app
CMD ["npm", "start"]