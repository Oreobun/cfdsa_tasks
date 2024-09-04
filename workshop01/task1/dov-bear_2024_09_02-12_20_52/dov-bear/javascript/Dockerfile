FROM node:22


### Create a directory 
WORKDIR /app

COPY main.js .
COPY package.json .
COPY public public
COPY views views 

### Set the env variable with name APP_PORT.
ENV APP_PORT=3000
ENV INSTANCE_NAME="bear bear"
ENV INSTANCE_HASH="bear hash"

EXPOSE ${APP_PORT}

### Install node modules.
RUN npm install

ENTRYPOINT node main 