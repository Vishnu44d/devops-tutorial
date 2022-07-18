{{ 18th July, 2022 }}
# Terms used commonly
- repositories
- images
- containers
- volume
- network
- Dockerfile
- docker-compose


# Images
- diff between images and containers
- naming convention - <repository/name>:tag (by deafult latest tag and dockerhub repo)
- images pull
```bash
sudo docker pull percona:8.0
```
- image layers
- Entrypoint

# Containers
- get all running containers
```bash
sudo docker ps
```
- get all containers
```bash
sudo docker ps -a
```
- run a container in interative mode (-it )
```bash
sudo docker run -it ubuntu:18.04 /bin/sh
```

- run a container in daemon mone (-d)
```bash
sudo docker run -d ubuntu:18.04 /bin/sh
```

- see logs of a container (69e242087be2 =  container_id)
```bash 
sudo docker logs 69e242087be2 
```

- follow a log
```bash
sudo docker logs 69e242087be2 -f
```

- Go into a container. exec into container
```bash
sudo docker exec -it 69e242087be2 /bin/bash
```

- Stop a container 
```bash
sudo docker stop 69e242087be2
```

- Remove a conatiner
```bash
sudo docker rm 69e242087be2
```

