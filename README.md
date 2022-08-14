## node-docker-webapp
In this repo created the restful api using node, express js and docker

## Links
- [Nodejs Docker Webapp/](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/)

# CMD
```sh
mkdir docker_web_app
cd docker_web_app 
touch package.json
touch server.js
touch Dockerfile
touch .dockerignore
```

```sh
docker build . -t pritamkhose/node-web-app

docker run -p 49160:8080 -d pritamkhose/node-web-app

docker images
docker ps
docker logs <container id> or docker logs 79703994a3ca
docker exec -it <container id> /bin/bash
docker kill <container id> or docker kill 79703994a3ca
```

# Example
Running on [http://localhost:8080](http://localhost:8080) or [http://localhost:49160/](http://localhost:49160/)

```sh
curl -i localhost:49160
```
