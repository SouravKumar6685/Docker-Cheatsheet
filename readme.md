

# 🐋 Docker Cheat Sheet 🚀  

<div style="color: #2E86C1; background-color: #EBF5FB; padding: 10px; border-radius: 5px; margin-bottom: 15px;">
<strong>🚀 Basic Container Commands</strong>
</div> 

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

<div style="color: #28B463; background-color: #EAFAF1; padding: 10px; border-radius: 5px; margin: 15px 0;">
<strong>📦 Image Management</strong>
</div> 

| Command | Description |
|---------|-------------|
| `docker images` | List all images |
| `docker pull nginx` | Pull an image from Docker Hub |
| `docker rmi nginx` | Remove an image |
| `docker image prune` | Remove all unused images |
| `docker build -t my-node-app .` | Build an image from a Dockerfile |

---

<div style="color:rgb(99, 124, 214); background-color:rgb(234, 249, 250); padding: 10px; border-radius: 5px; margin: 15px 0;">
<strong>🏃Running Containers </strong>
</div>

| Command | Description |
|---------|-------------|
| `docker run -it ubuntu /bin/bash` | Run a container interactively |
| `docker run -d nginx` | Run a container in detached mode |
| `docker run --name django-app django` | Run a container with a specific name |
| `docker run -p 3000:3000 my-react-app` | Run a container with port mapping |
| `docker run -v /my/local/path:/app my-node-app` | Run a container with a mounted volume |

---

<div style="color:rgb(99, 124, 214); background-color:rgb(247, 234, 250); padding: 10px; border-radius: 5px; margin: 15px 0;">
<strong>📂 4. Volumes & Storage </strong>
</div>

| Command | Description |
|---------|-------------|
| `docker volume ls` | List all volumes |
| `docker volume create my_volume` | Create a volume |
| `docker volume rm my_volume` | Remove a volume |
| `docker volume prune` | Remove all unused volumes |
| `docker run -v my_volume:/data postgres` | Mount a volume when running a container |

---

<div style="color:rgb(99, 124, 214); background-color:rgb(246, 250, 234); padding: 10px; border-radius: 5px; margin: 15px 0;">
<strong>🌐 5. Networking </strong>
</div>

| Command | Description |
|---------|-------------|
| `docker network ls` | List all networks |
| `docker network create my_network` | Create a network |
| `docker network connect my_network django-app` | Connect a container to a network |
| `docker network disconnect my_network django-app` | Disconnect a container from a network |
| `docker network rm my_network` | Remove a network |

---

<div style="color:rgb(99, 124, 214); background-color:rgb(250, 242, 234); padding: 10px; border-radius: 5px; margin: 15px 0;">
<strong>📝 6. Docker Compose </strong>
</div>

| Command | Description |
|---------|-------------|
| `docker-compose up -d` | Start services using `docker-compose.yml` |
| `docker-compose down` | Stop services |
| `docker-compose restart` | Restart services |
| `docker-compose logs -f` | View logs |

---


<div style="color:rgb(99, 124, 214); background-color:rgb(246, 250, 234); padding: 10px; border-radius: 5px; margin: 15px 0;">
<strong>🔍 7. Debugging & Monitoring </strong>
</div>

| Command | Description |
|---------|-------------|
| `docker logs my_container` | View logs of a container |
| `docker top my_container` | View running processes inside a container |
| `docker inspect my_container` | Inspect container details |
| `docker exec -it <ID> sh` | Enter running container |
| `docker stats` | Show container resource usage |

---

<div style="color:rgb(99, 124, 214); background-color:rgb(250, 234, 234); padding: 10px; border-radius: 5px; margin: 15px 0;">
<strong>🔥 8. Cleaning Up </strong>
</div>

| Command | Description |
|---------|-------------|
| `docker container prune` | Remove all stopped containers |
| `docker image prune -a` | Remove all unused images |
| `docker network prune` | Remove all unused networks |
| `docker volume prune` | Remove all unused volumes |
| `docker system prune -a` | Remove **everything** (containers, images, networks, volumes) |




