# Specifies base image
FROM node:14-alpine

# Copy files from host to container
WORKDIR /usr/app
COPY ./package.json ./

# Install dependencies
RUN npm install

COPY ./ ./

# Default command
CMD ["npm", "start"]