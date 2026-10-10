
# Mission 6: The Cloud Deployment Engineer — Reflection

This laboratory activity helped me understand how Docker Compose makes deploying cloud applications easier and more organized. Before this mission, I thought that deploying an application required manually creating and configuring each container separately. By writing a `docker-compose.yml` file, I learned that I could define multiple services in one configuration and deploy them together using a single command. This approach saves time, reduces repetitive work, and makes the deployment easier to reproduce.

I also learned that YAML indentation is very important. If I accidentally use a Tab instead of spaces or place a line at the wrong indentation level, Docker Compose may fail to read the configuration correctly. This taught me to be careful when writing configuration files and to check my code before running it.

Environment variables, such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_HOST`, help configure the application and establish communication between Nextcloud and MariaDB. They allow the containers to use the correct database credentials and connection information without putting these settings directly into application code. However, I also learned that passwords written directly in a Compose file are not suitable for production environments because they can be exposed. More secure methods should be used for real deployments.

Deploying Nextcloud was an exciting learning experience because it showed me how a private cloud storage application can be prepared using only a few commands. It helped me appreciate how different components work together to provide a useful service. I also realized that successful deployment requires more than starting containers; testing, monitoring, security, and documentation are important.

Since Mission 1, my understanding of cloud computing has developed from learning basic concepts to understanding how actual infrastructure can be configured and managed. I now have a better appreciation of containers, service communication, and Infrastructure as Code. This mission encouraged me to continue practicing Linux commands, Docker, and cloud deployment so I can improve my skills as a future IT professional.
