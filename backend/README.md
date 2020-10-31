## Project setup:

### Build Docker Image and Push to DockerHub
```
sudo docker build .
sudo docker tag 2887cd8c3c37 harryyao/dailydash:v1
sudo docker push harryyao/dailydash:v1
```

### Deploy Docker Image
```
sudo docker pull harryyao/dailydash:v1
sudo docker ps
sudo docker run [Container ID] -P -d
```