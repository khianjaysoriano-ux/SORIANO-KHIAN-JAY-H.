
# Docker Compose Guide

## 1. What Does the `services:` Block Do?

The `services:` block defines the containers that make up the application. In this project, it defines two services: `database`, which runs MariaDB 10.6, and `app`, which runs Nextcloud. Docker Compose uses these definitions to create and manage the application services together.

## 2. How Does Nextcloud Find the Database?

The Nextcloud application uses the `MYSQL_HOST=database` environment variable to locate the database service. Docker Compose provides service-name-based network communication between containers on the same project network. Therefore, Nextcloud can use the hostname `database` instead of requiring a fixed IP address.

## 3. Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is generally used to create and start an individual container with options supplied on the command line. Docker Compose reads a YAML configuration file and manages multiple related services together. The `docker-compose up -d` command deploys the defined services in the background, making multi-container applications easier to configure, repeat, and maintain.

## 4. Infrastructure as Code (IaC)

Infrastructure as Code means defining infrastructure using readable configuration files instead of relying entirely on manual setup. The `docker-compose.yml` file acts as a blueprint for the Nextcloud and MariaDB services. It makes the deployment easier to reproduce and helps reduce mistakes caused by repeatedly entering commands manually.

## 5. Commands Used

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
cat docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose logs app
docker-compose logs database
docker-compose down
```

## 6. Conclusion

Docker Compose simplifies the deployment and management of multi-container applications. By defining Nextcloud and MariaDB in one configuration file, a cloud engineer can deploy, inspect, and remove the application stack with a small set of commands.
