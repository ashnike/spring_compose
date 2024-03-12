# Docker Compose Project
## Architecture diagram
![](https://github.com/ashnike/spring_compose/blob/main/new.GIF)

This repository contains a Docker Compose setup for a Java web application along with a MySQL database and Nginx web server. The structure of the repository is organized as follows:

## Directory Structure

- **app**: Contains the Java web application source code.
  - **Dockerfile**: Dockerfile for building the Java application image.
  - **pom.xml**: Maven project configuration file.
  - **src**: Source code directory.
- **db**: Contains the MySQL database configuration.
  - **db_backup.sql**: Initial SQL script to populate the database.
  - **Dockerfile**: Dockerfile for building the MySQL database image.
- **web**: Contains the Nginx web server configuration.
  - **Dockerfile**: Dockerfile for building the Nginx image.
  - **nginxjapp.conf**: Nginx configuration file.
  - **docker-compose.yml**: Docker Compose configuration file.
## Usage

To run the entire application stack using Docker Compose, follow these steps:

1. Make sure you have Docker and Docker Compose installed on your system.

2. Clone this repository to your local machine:
```
   git clone https://github.com/ashnike/spring_compose.git
```
3. Run the following command to build and start the Docker containers:
```
   docker-compose up -d
``` 
