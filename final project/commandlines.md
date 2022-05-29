

Build the image 
```shell
docker build -t ic-webapp:1.0 .
```

Create the container instance 
```shell
docker run --name test-ic_webapp -d -p 8080:8080 ic-webapp:1.0 
```

Push the image into the docker hub
```shell
XXXX
```

### History 



```shell
docker login
docker tag f9551d77ee45 eha3112dockerhub/ic-webapp:1.0
docker push eha3112dockerhub/ic-webapp:1.0 
```

### Usefull commands 
```shell
docker logs <CONTAINER ID/NAME>
```

```shell
docker image ls
```

```shell
docker ps
```

```shell
docker logs test-ic_webapp
```

```shell
docker container kill <CONTAINER ID/NAME>
```

```shell
docker rmi -f <IMAGE ID>
```

Delete all containers (working/stopped)
```shell
docker rm -f $(docker ps -a -q)
```

Delete all images
```shell
docker rmi -f $(docker images -aq)
```

### How to to docker hub
1. Connect to Docker hub using your docker hub Id and password 
```shell
docker login
```
2. tag the image in a particular format (docker hub Id/image name:version)
```shell
docker tag <IMAGE ID> <docker hub Id>/name:version
```
3. push the new image 
```shell
docker push REPOSITORY/TAG
```


