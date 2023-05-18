FROM node:latest

WORKDIR /app

RUN npm install json-server

COPY db.json /app/db.json

EXPOSE 3000

ENTRYPOINT [ "npx", "json-server", "db.json", "--host", "0.0.0.0"]