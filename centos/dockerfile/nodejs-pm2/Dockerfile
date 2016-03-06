FROM node:latest
MAINTAINER cowpanda

RUN npm install -g pm2@latest

VOLUME ["/app"]
ADD start /start
RUN chmod 755 /start
CMD ["/start"]

EXPOSE 10000-10100
