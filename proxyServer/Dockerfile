# MAINTAINER stacy.chen@fuhu.com

FROM gradle:4.2.1-jdk8-alpine
WORKDIR /proxyServer
ADD . /proxyServer

# change role to let gradle run
USER root
RUN chown -R gradle /proxyServer
USER gradle

RUN gradle
RUN gradle build -x test
EXPOSE 8080
CMD ["java", "-jar", "build/libs/gateway-0.0.1-SNAPSHOT.jar"]
