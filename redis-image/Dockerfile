# use the existing docker image as base
FROM alpine

# download and install the dependencies
RUN apk add --update redis
RUN apk add --update gcc

# Tell the image what to do when it starts as a containser 
CMD ["redis-server"]