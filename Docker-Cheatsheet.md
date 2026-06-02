# 🐳 Docker Cheat Sheet for DevOps Engineers

A practical Docker command reference for DevOps Engineers, Cloud Engineers, SREs, and Developers.

---

# Verify Docker Installation

```bash
docker --version
docker info
```

---

# Docker Images

## Download an Image

```bash
docker pull nginx
docker pull ubuntu:22.04
```

## List Images

```bash
docker images
```

## Inspect Image

```bash
docker inspect nginx
```

## Build Image

```bash
docker build .
docker build -t myapp:v1 .
```

## Build from Git Repository

```bash
docker build https://github.com/docker/rootfs.git#container:docker
```

## Tag Image

```bash
docker tag myapp:v1 myrepo/myapp:v1
```

## Push Image

```bash
docker push myrepo/myapp:v1
```

## Remove Image

```bash
docker rmi image_id
docker rmi nginx
```

## Remove Unused Images

```bash
docker image prune
```

---

# Docker Containers

## Run Container

```bash
docker run nginx
```

## Run Container in Detached Mode

```bash
docker run -d nginx
```

## Run Interactive Container

```bash
docker run -it ubuntu bash
```

## Run with Custom Name

```bash
docker run --name web nginx
```

## Run and Expose Port

```bash
docker run -p 8080:80 nginx
```

## Run with Environment Variable

```bash
docker run -e ENV=prod nginx
```

## Run with Volume Mapping

```bash
docker run -v /host/path:/container/path nginx
```

## Auto Remove Container

```bash
docker run --rm nginx
```

---

# List Containers

## Running Containers

```bash
docker ps
```

## All Containers

```bash
docker ps -a
```

---

# Start, Stop & Restart Containers

## Start Container

```bash
docker start container_name
```

## Stop Container

```bash
docker stop container_name
```

## Restart Container

```bash
docker restart container_name
```

## Kill Container

```bash
docker kill container_name
```

## Pause Container

```bash
docker pause container_name
```

## Unpause Container

```bash
docker unpause container_name
```

---

# Container Logs

## View Logs

```bash
docker logs container_name
```

## Follow Logs

```bash
docker logs -f container_name
```

## Last 50 Lines

```bash
docker logs --tail 50 container_name
```

---

# Access Running Container

## Open Shell

```bash
docker exec -it container_name bash
```

## Execute Command

```bash
docker exec container_name ls
```

## Attach to Running Container

```bash
docker attach container_name
```

---

# Inspect Resources

## Container Details

```bash
docker inspect container_name
```

## Live Resource Usage

```bash
docker stats
```

## Process List

```bash
docker top container_name
```

---

# Remove Containers

## Remove Stopped Container

```bash
docker rm container_name
```

## Force Remove

```bash
docker rm -f container_name
```

## Remove Container and Volume

```bash
docker rm -v container_name
```

---

# Docker Volumes

## Create Volume

```bash
docker volume create myvolume
```

## List Volumes

```bash
docker volume ls
```

## Inspect Volume

```bash
docker volume inspect myvolume
```

## Remove Volume

```bash
docker volume rm myvolume
```

## Remove Unused Volumes

```bash
docker volume prune
```

---

# Docker Networks

## Create Network

```bash
docker network create devops-net
```

## List Networks

```bash
docker network ls
```

## Inspect Network

```bash
docker network inspect devops-net
```

## Connect Container to Network

```bash
docker network connect devops-net container_name
```

## Disconnect Container

```bash
docker network disconnect devops-net container_name
```

## Delete Network

```bash
docker network rm devops-net
```

---

# Docker Compose

## Start Services

```bash
docker compose up
```

## Start in Background

```bash
docker compose up -d
```

## Stop Services

```bash
docker compose down
```

## View Logs

```bash
docker compose logs
```

## Restart Services

```bash
docker compose restart
```

## List Services

```bash
docker compose ps
```

---

# Docker System Cleanup

## Remove Unused Objects

```bash
docker system prune
```

## Remove Everything

```bash
docker system prune -a
```

## Check Docker Disk Usage

```bash
docker system df
```

---

# Docker Registry Commands

## Login

```bash
docker login
```

## Logout

```bash
docker logout
```

## Search Images

```bash
docker search nginx
```

---

# Docker Swarm Commands

## Initialize Swarm

```bash
docker swarm init
```

## Join Swarm

```bash
docker swarm join
```

## List Services

```bash
docker service ls
```

## Create Service

```bash
docker service create nginx
```

## Scale Service

```bash
docker service scale myservice=5
```

## Update Service

```bash
docker service update myservice
```

---

# Most Important Commands for Interviews

```bash
docker pull nginx
docker images
docker build -t myapp:v1 .
docker run -d -p 8080:80 nginx
docker ps -a
docker logs -f container_name
docker exec -it container_name bash
docker stop container_name
docker rm container_name
docker rmi nginx
docker volume ls
docker network ls
docker compose up -d
docker system prune -a
```


⭐ If this repository helps you, give it a star.
