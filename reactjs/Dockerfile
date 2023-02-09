# Base Image
FROM node:lts-alpine

# Working Directory (WORKDIR)
WORKDIR /usr/app

# Copy package.json 
COPY ./package.json ./

# Clean npm cache
RUN npm cache clean --force

# Run Command
RUN npm install --force

# Copy code from host to container
COPY ./ ./

# Default Command
CMD [ "npm", "start" ]