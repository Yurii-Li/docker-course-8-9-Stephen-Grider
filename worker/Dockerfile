# 1. docker build -t complex:worker .
# 2. docker run -p 3000:3000 complex:worker

FROM node:lts-alpine

WORKDIR "/app"

COPY ./package.json ./

RUN npm install

COPY . .

CMD ["npm", "run", "start"]