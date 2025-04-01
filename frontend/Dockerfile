FROM node:15.14-alpine

WORKDIR /app

EXPOSE 3000

COPY package.json package-lock.json ./

RUN npm install --silent
RUN npm uninstall react-scripts
RUN npm install react-scripts

COPY . ./

CMD ["npm", "start"]