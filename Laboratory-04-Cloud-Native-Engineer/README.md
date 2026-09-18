
# Laboratory 04 – The Cloud-Native Engineer

## Mission Overview

Laboratory Activity 4 focuses on cloud-native engineering and containerization. The activity demonstrates the difference between traditional Virtual Machines and containers and provides practical experience using Docker. Using the KillerCoda Playground, an Nginx web server was downloaded, deployed, tested, stopped, and removed.

## Objectives

* Differentiate Virtual Machines from containers.
* Access a Docker-enabled Linux environment.
* Execute fundamental Docker CLI commands.
* Pull and run an Nginx container.
* Map a host port to a container port.
* Manage the container lifecycle.
* Document Docker operations using Markdown.
* Maintain an organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Docker Verification

```bash
docker --version
docker info
```

### Nginx Deployment

```bash
docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx
docker ps
curl http://localhost:8080
```

### Container Lifecycle

```bash
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a
```

## Skills Learned

* Docker CLI usage
* Container deployment
* Nginx deployment
* Port mapping
* Container lifecycle management
* Linux terminal operations
* Technical documentation
* Markdown documentation
* GitHub portfolio management

## Challenges Encountered

One challenge I encountered was understanding the difference between a virtual machine and a container. I also needed to become familiar with Docker commands and understand how port mapping connects the host machine to a service running inside a container. Another challenge was making sure that each command was executed in the correct order and that screenshots were captured as evidence. Through practice, I became more comfortable using the Docker CLI and managing containers.
