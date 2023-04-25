FROM node:18-alpine 


WORKDIR /front


COPY package*.json ./


RUN npm install



COPY ./public ./public

COPY ./src/ app

RUN npm run build


EXPOSE 8081


CMD ["npm", "start"]
