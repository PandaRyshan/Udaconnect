FROM node:18-alpine

WORKDIR .

COPY package.json ./
COPY package-lock.json ./

RUN npm install
RUN npm install react-scripts@5.0.1 -g
RUN npx update-browserslist-db@latest

CMD ["pwd"]
COPY . ./

EXPOSE 3000

CMD ["npm", "start"]

