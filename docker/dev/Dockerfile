# Install base image fronm nodeJS v14
FROM node:14-alpine
# Set Environment variable
ENV NODE_ENV development
# Install dependencies
RUN apk update
RUN apk add git
# Set user to the current host user
USER 1000
# Set current directory to /app
WORKDIR /app
# Copy packages files
COPY --chown=1000:1000 package.json .
COPY --chown=1000:1000 package-lock.json .

ENTRYPOINT [ "/app/entrypoint.sh" ]
# Expose port
EXPOSE 3000
CMD [ "npm", "start" ]
