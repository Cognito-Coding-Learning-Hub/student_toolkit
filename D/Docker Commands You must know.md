🐳 Docker Must-Know Command Cheat Sheet (No Hyphen in compose)
📦 Containers – Lifecycle

docker ps                      # List running containers
docker ps -a                   # List all containers (including stopped)
docker run -it ubuntu bash     # Run a container interactively
docker run -d nginx            # Run a container in the background
docker start <container_id>    # Start a stopped container
docker stop <container_id>     # Stop a running container
docker restart <container_id>  # Restart a container
docker rm <container_id>       # Remove a container
docker logs <container_id>     # View container logs
docker exec -it <container_id> bash  # Get a shell inside container
docker inspect <container_id>  # Detailed info about container
docker stats                   # Live CPU/memory usage

📦 Images

docker images                  # List local images
docker pull ubuntu             # Download image from Docker Hub
docker build -t myimage .      # Build image from Dockerfile in current dir
docker rmi <image_id>          # Remove image
docker tag <image_id> myrepo/myimage:latest  # Tag image
docker push myrepo/myimage:latest           # Push image to registry

🗂 Volumes

docker volume ls               # List volumes
docker volume create myvol     # Create volume
docker volume inspect myvol    # Inspect volume
docker run -v myvol:/data ubuntu # Mount volume in container
docker volume rm myvol         # Remove volume

🌐 Networks

docker network ls              # List networks
docker network create mynet    # Create network
docker network inspect mynet   # Inspect network
docker network connect mynet <container_id>  # Connect container
docker network disconnect mynet <container_id> # Disconnect

⚙️ Docker Compose (New Syntax)

👉 You said you’re on the version with no hyphen:
✅ Use: docker compose
🚫 Not: docker-compose

docker compose up              # Start services defined in docker-compose.yml
docker compose up -d           # Start services in detached mode
docker compose down            # Stop and remove containers, networks
docker compose restart         # Restart all services
docker compose ps              # List services/containers
docker compose logs            # Show logs from services
docker compose logs -f         # Follow logs
docker compose build           # Build or rebuild services
docker compose pull            # Pull images defined in compose file
docker compose exec service bash  # Exec into a running service container
docker compose stop            # Stop services
docker compose start           # Start services

🔧 Cleaning Up

docker system prune            # Remove unused containers, networks, images
docker container prune         # Remove all stopped containers
docker image prune             # Remove unused images
docker volume prune            # Remove unused volumes
docker network prune           # Remove unused networks

📌 Tips

✅ Use docker ps --format "{{.Names}}: {{.Status}}" for cleaner output
✅ Combine docker exec with bash or sh for debugging containers
✅ Always docker compose down before modifying your compose file
