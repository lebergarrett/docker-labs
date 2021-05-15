# Specify a base image
FROM node:alpine

# Set up working directory for container (where files will be stored)
WORKDIR /usr/app

# Move file listing dependencies from host into container
COPY ./package.json ./

# Install some dependencies
RUN npm install

# Copy the rest of the files into container
COPY ./ ./

# Default command
CMD ["npm", "start"]