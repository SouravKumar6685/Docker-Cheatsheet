

# 🐋 Docker Cheat Sheet 🚀  

## 🚀 Basic Container Commands

| Command | Description |
|---------|-------------|
| `docker --version` | Check Docker version |
| `docker ps` | List running containers |
| `docker ps -a` | List all containers (including stopped ones) |
| `docker start my_container` | Start a stopped container |
| `docker stop my_container` | Stop a running container |
| `docker restart my_container` | Restart a container |
| `docker rm my_container` | Remove a container |
| `docker container prune` | Remove all stopped containers |

---

## 📦 Image Management

| Command | Description |
|---------|-------------|
| `docker images` | List all images |
| `docker pull nginx` | Pull an image from Docker Hub |
| `docker rmi nginx` | Remove an image |
| `docker image prune` | Remove all unused images |
| `docker build -t my-node-app .` | Build an image from a Dockerfile |

---

## 🏃Running Containers

| Command | Description |
|---------|-------------|
| `docker run -it ubuntu /bin/bash` | Run a container interactively |
| `docker run -d nginx` | Run a container in detached mode |
| `docker run --name django-app django` | Run a container with a specific name |
| `docker run -p 3000:3000 my-react-app` | Run a container with port mapping |
| `docker run -v /my/local/path:/app my-node-app` | Run a container with a mounted volume |

---

## 📂 4. Volumes & Storage

| Command | Description |
|---------|-------------|
| `docker volume ls` | List all volumes |
| `docker volume create my_volume` | Create a volume |
| `docker volume rm my_volume` | Remove a volume |
| `docker volume prune` | Remove all unused volumes |
| `docker run -v my_volume:/data postgres` | Mount a volume when running a container |

---

## 🌐 5. Networking

| Command | Description |
|---------|-------------|
| `docker network ls` | List all networks |
| `docker network create my_network` | Create a network |
| `docker network connect my_network django-app` | Connect a container to a network |
| `docker network disconnect my_network django-app` | Disconnect a container from a network |
| `docker network rm my_network` | Remove a network |

---

## 📝 6. Docker Compose

| Command | Description |
|---------|-------------|
| `docker-compose up -d` | Start services using `docker-compose.yml` |
| `docker-compose down` | Stop services |
| `docker-compose restart` | Restart services |
| `docker-compose logs -f` | View logs |

---


## 🔍 7. Debugging & Monitoring 

| Command | Description |
|---------|-------------|
| `docker logs my_container` | View logs of a container |
| `docker top my_container` | View running processes inside a container |
| `docker inspect my_container` | Inspect container details |
| `docker exec -it <ID> sh` | Enter running container |
| `docker stats` | Show container resource usage |

---

## 🔥 8. Cleaning Up 

| Command | Description |
|---------|-------------|
| `docker container prune` | Remove all stopped containers |
| `docker image prune -a` | Remove all unused images |
| `docker network prune` | Remove all unused networks |
| `docker volume prune` | Remove all unused volumes |
| `docker system prune -a` | Remove **everything** (containers, images, networks, volumes) |




