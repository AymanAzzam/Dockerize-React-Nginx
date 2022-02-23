# Install base image fronm nodeJS v14
FROM node:14-alpine
# Set Environment variable
ENV NODE_ENV production
# Install dependencies
RUN apk --no-cache add git
# Add a work directory
WORKDIR /app
# Copy app files
COPY package.json .
COPY package-lock.json .
# Install packages
RUN npm install
# Expose port
EXPOSE 3000
