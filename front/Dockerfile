# Use an official Node.js runtime as a parent image
FROM node:18-alpine

# Set the working directory to /app
RUN mkdir -p usr/src/app

WORKDIR /usr/src/app

COPY package.jason /usr/src/app

RUN npm install

ADD src /usr/src/app/src

ADD public /usr/src/app/public

RUN npm build 

EXPOSE 8081 

CMD ["npm","start"]

