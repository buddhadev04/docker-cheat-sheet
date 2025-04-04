# 🐳 Docker Cheat Sheet

A simple, comprehensive cheat sheet to help you work efficiently with Docker.

---

## 🧰 Basic Commands

```bash
docker version                              # Check Docker version
docker info                                 # Display system-wide info
docker pull <image>                         # Pull image from registry
docker images                               # List all images
docker rmi <image>                          # Remove image
docker ps                                   # List running containers
docker ps -a                                # List all containers
docker stop <container>                     # Stop a container
docker start <container>                    # Start a container
docker restart <container>                  # Restart a container
docker rm <container>                       # Remove a container
docker logs <container>                     # View container logs
docker exec -it <container> /bin/bash       # Access container shell

# Running Containers

docker run <image>                          # Run container from image
docker run -d <image>                       # Run in detached mode
docker run -p 8080:80 <image>               # Map port (host:container)
docker run -v /host:/container <image>      # Mount volume
docker run --name <name> <image>            # Name a container
docker run -e VAR=value <image>             # Set environment variable
docker run --rm <image>                     # Auto-remove after stopping


# Docker Compose

docker-compose up                           # Start services
docker-compose up -d                        # Start in background
docker-compose down                         # Stop and remove services
docker-compose build                        # Build or rebuild services
docker-compose ps                           # List containers
docker-compose logs                         # View service logs
docker-compose restart                      # Restart services

# Container Management

docker inspect <container>                  # Detailed container info
docker stats                                # Container resource usage
docker top <container>                      # Processes in container
docker port <container>                     # View port mappings
docker cp <container>:/path /host           # Copy files from container


