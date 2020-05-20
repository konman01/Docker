# define the base image
FROM node:alpine

WORKDIR '/app'
COPY package.json .

# Install all the dependencies required
RUN npm install

COPY . .

# Start up command
CMD ["npm", "start"]