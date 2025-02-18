FROM ubuntu:latest
LABEL authors="MrFlava"

ENTRYPOINT ["top", "-b"]

FROM node:23-alpine

RUN npm install -g nodemon

WORKDIR /app

COPY . .

RUN npm install

EXPOSE 4000

CMD ["npm", "run", "dev"]