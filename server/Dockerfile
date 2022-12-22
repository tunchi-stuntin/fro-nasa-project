FROM node:14

WORKDIR /server

COPY package.json ./

RUN npm i && \
    npm install husky && \
    npm audit fix

COPY . .

EXPOSE 8000

CMD [ "npm", "start"]