# Dockerfile !

# Pull the official base image
FROM node:16.2-alpine

# set working directory
WORKDIR /app

# copy package.json and package-lock.json into the container
COPY package*.json .

# install dependencies
RUN npm install 

# copy the rest of the application into the container
COPY . . 

# expose the application on port 3000
EXPOSE 3000

# start the application when the container is running
CMD [ "npm" , "start" ]