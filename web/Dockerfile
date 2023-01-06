FROM node:16-slim

RUN groupadd -g 1009 workshop && useradd -r -u 1009 -g workshop workshop
USER workshop

# Create app directory
WORKDIR /usr/src/app

# Bundle app source
COPY . .

EXPOSE 8080
CMD [ "node", "server.js" ]
