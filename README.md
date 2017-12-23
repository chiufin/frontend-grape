# Introduction
Using zuul to set proxyServer, route to f2eServer

ref: [Sprint Cloud](http://projects.spring.io/spring-cloud/)
### Develop
1. cd /f2eServer
```
node server
```
* run on `http://localhost:8090/`

ref: next.js + redux + figure

2. cd /proxyServer
```
gradle build
java -jar build/bins/xxx.jar
```
* run on `http://localhost:8080/hello/`

ref: java 8

## Deploy with Docker
```
docker build -t grape-f2e-server .
docker run -p 8090:8090
```

```
docker build -t grape-proxy-server .
docker run -p 8080:8080 grape-proxy-server
```