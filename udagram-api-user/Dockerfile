FROM node:12
#create app directory
WORKDIR /usr/src/app
#install app dependencies
#ensure package.json and package-lock.json are both copied
COPY package*.json ./

RUN npm.ci
#bundle app source
COPY . .
EXPOSE 8000
CMD [ "npm", "run", "prod"]