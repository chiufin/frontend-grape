# MAINTAINER stacy.chen@fuhu.com
FROM node:6.12.2-alpine
WORKDIR /f2eServer

ADD ./ /f2eServer
RUN npm install
EXPOSE 8090
CMD ["node", "server"]
