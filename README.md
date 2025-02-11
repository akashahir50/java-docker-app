
# java-docker

A brief description of what this project does and who it's for


## Deployment

To updates the package lists of the system to ensure you have the latest information about available packages.

```bash
 sudo apt-get update
```
Installs the Docker Engine on the system
```bash
 sudo apt-get install docker.io
```
Checks the status of the Docker service to verify if it's running correctly
```bash
 sudo systemctl status docker
```
Adds the current user to the docker group, granting them necessary permissions to interact with Docker without root privileges
```bash
 sudo usermod -aG docker $USER
```
Refreshes the user's group memberships, allowing the changes made by usermod to take effect immediately
```bash
 newgrp docker
```
Lists all running Docker containers
```bash
 docker ps
```
Lists all Docker images available on the local machine
```bash
 docker images
```
Authenticates with a Docker registry (e.g., Docker Hub) to push and pull images
```bash
 docker login 
```
Downloads the official MySQL image from Docker Hub
```bash
 docker pull mysql
```
Starts a detached MySQL container, setting the root password for the database
```bash
 docker run -d -e MYSQL_ROOT_PASSWORD=root mysql
```
Creates a new directory named "projects" to organize your projects
```bash
 mkdir projects
```
Changes the current directory to the "projects" directory
```bash
 cd projects
```
Clones your Git repository from the specified URL into the "projects" directory
```bash
 git clone {your git repo link here}
```
Lists the contents of the current directory
```bash
 ls
```
Changes the current directory into the cloned project directory
```bash
 cd java-docker-app-project
```
Lists the contents of the "java-docker-app-project" directory
```bash
 ls
```
Opens the Dockerfile for editing using the vim text editor
```bash
 vim Dockerfile 
```
Builds a Docker image from the Dockerfile and tags it as "java-app"
```bash
 docker build -t java-app .
```
Lists the Docker images, including the newly built "java-app" image
```bash
 docker images
```
Runs a container using the "java-app" image
```bash
  docker run java-app
```

