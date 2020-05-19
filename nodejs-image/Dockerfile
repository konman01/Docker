# specify a base image
#FROM alpine -- this image does not have node
# so used the below base having node
FROM node:alpine

# Any following commanmd will be executed relative
# to this path in the container
WORKDIR /usr/app

# copy all the files from the current dir of localhost
# unnecessary build happens if we change the index.js file
# COPY ./ ./

# by this approch if we change the index.js file any  time, then rebuild is not required
COPY ./package.json ./
RUN npm install
COPY ./ ./

# install some dependencies
RUN npm install

# Default command to execute
CMD ["npm", "start"]