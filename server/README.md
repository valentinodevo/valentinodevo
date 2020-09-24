# single-line web-server using bash


To build server into docker-image and save docker-image to docker hub:
```
docker build --tag valentinodevo/server:stable .
docker push valentinodevo/server:stable
```

Example of command with defined port and message to run server and test work of it:
```
$ docker run -it  -p 80:8081 -d  valentinodevo/server:stable  8081 TestServer-OK
dd38d8cccc28d2e5a4103d393a035f8844093472b9d749929023b1c68394bcd2
$ curl localhost:80
TestServer-OK
```

Example of command with default values to run server and test work of it:
```
$ docker run -it  -p 8088:80 -d  valentinodevo/server:stable
cfedef0c3b305fcfd3e684ffb73c2bf1f7d6b91399c736e01dab3adef97ee201
$ curl 127.0.0.1:8088
Test-OK
```
