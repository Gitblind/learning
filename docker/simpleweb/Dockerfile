#Specify a base image
FROM node:alpine

#Change the directory in docker
WORKDIR /usr/app

#Install some dependencies
COPY ./package.json ./
RUN npm install

#Copy source code to minimize rebuild
COPY ./ ./

#Default command run will call
CMD [ "npm", "start" ]