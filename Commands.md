

Docker Cheat Sheet



---
1. Images
---
docker pull <image> – Download an image

docker images – List all images

docker rmi <image> – Remove an image



---
2. Containers
---
docker run -d --name <container> <image> – Run a container in detached mode

docker ps – List running containers

docker ps -a – List all containers

docker stop <container> – Stop a container

docker rm <container> – Remove a container



---

3. Networking

docker network ls – List networks

docker network create <name> – Create a custom network

docker network inspect <name> – Inspect a network

docker network connect <network> <container> – Attach a container to a network



---

4. Volumes & Storage

docker volume create <name> – Create a volume

docker volume ls – List volumes

docker volume inspect <name> – Inspect a volume

docker run -v <volume>:/path <image> – Mount a volume



---

5. Docker Compose

docker-compose up -d – Start services in detached mode

docker-compose down – Stop and remove containers

docker-compose logs – View logs of all services



---

6. Building & Pushing Images

docker build -t <image>:<tag> . – Build an image

docker tag <image> <repo>/<image>:<tag> – Tag an image

docker push <repo>/<image>:<tag> – Push an image to a registry



---

7. Debugging & Logs

docker logs -f <container> – Follow logs of a running container

docker exec -it <container> /bin/sh – Access a running container

docker inspect <container> – Get detailed container information



---

Bonus Tip

Use multi-stage builds in Dockerfiles to keep your images lightweight and secure!


