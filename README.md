SeedStack hub is a social platform to discover and share software components.

This hub is using a Mongo Database. 

To run this image:
```
docker run -d -p 8080:8080 -e JAVA_OPTS="-DmongoHosts=<mongodb host>" seedstack/hub
```


If you use a proxy to connect to internet:
```
docker run -d -p 8080:8080 -e JAVA_OPTS="-DmongoHosts=<mongodb host>" 
-e http_proxy=$http_proxy -e https_proxy=$https_proxy -e no_proxy=$no_proxy seedstack/hub
```
