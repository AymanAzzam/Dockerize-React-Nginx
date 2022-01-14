# Install base image fronm nodeJS v14
FROM node:14-alpine
# Set Environment variable
ENV NODE_ENV production
# Install dependencies
# RUN apk update
# RUN apk add git
# Add a work directory
WORKDIR /app
# Copy app files
COPY package.json .
COPY package-lock.json .
RUN npm install
COPY . .
# Expose port
EXPOSE 3000
