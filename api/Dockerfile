FROM ubuntu:latest
LABEL authors="MrFlava"

ENTRYPOINT ["top", "-b"]

FROM node:23-alpine

WORKDIR /app

COPY . .

RUN npm install

EXPOSE 4000

CMD ["node", "app.js"]