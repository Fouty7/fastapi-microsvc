FROM node:18-alpine

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 10086
EXPOSE 8001
EXPOSE 443
EXPOSE 8000
EXPOSE 80

CMD ["npm", "start"]