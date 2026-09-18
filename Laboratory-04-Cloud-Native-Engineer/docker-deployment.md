
# Docker Deployment

## 1. Verify Docker Installation

```bash
docker --version
```

This command displays the installed Docker version and confirms that the Docker CLI is available.

```bash
docker info
```

This command displays information about the Docker environment and confirms that the Docker daemon is responding.

## 2. Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image from Docker Hub to the local Docker environment.

## 3. Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command creates and starts an Nginx container in detached mode and maps host port 8080 to container port 80.

## 4. List Running Containers

```bash
docker ps
```

This command displays the containers that are currently running.

## 5. Test the Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx server through port 8080 and verifies that the web server is responding.

## 6. Stop the Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

## 7. Verify the Container Is Stopped

```bash
docker ps -a
```

This command displays all containers, including stopped containers, allowing the user to verify that nginx-server is no longer running.

## 8. Remove the Container

```bash
docker rm nginx-server
```

This command permanently removes the stopped Nginx container from the Docker environment.

## 9. Verify Removal

```bash
docker ps -a
```

This command verifies that the nginx-server container has been removed.
