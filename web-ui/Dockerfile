FROM node:latest as builder

MAINTAINER Aayushi Raval <araval3@horizon.csueastbay.edu>

# Create directory for web-ui
RUN mkdir /web-ui
WORKDIR /web-ui

# Install npm modules before copying src code
# (so we have a Docker's caching layer for node_modules)
COPY package.json /web-ui/package.json
COPY package-lock.json /web-ui/package-lock.json
RUN npm --engine-strict=true ci

# Copy src code to image
COPY . /web-ui

EXPOSE 3000
ENTRYPOINT npm run start