---
title: Docker CLI Cheatsheet
layout: default
has_children: false
parent: Containerization
nav_order: 3
---

# Docker CLI Cheatsheet
{: .no_toc }

Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}

---

### Docker Images

Build an Image from a Dockerfile
   ```
   docker build -t <image_name>
   ```

Build an Image from a Dockerfile without Cache
   ```
   docker build -t <image_name> -no-cache
   ```

List Images
   ```
   docker images
   ```

Search for an Image
   ```
   docker search <image_name>
   ```

Remove an Image
   ```
   docker rmi <image_name>
   ```

### Docker Hub

Login to Docker Hub
   ```
   docker login - u <username>
   ```

Logout from Docker Hub
   ```
   docker logout
   ```

Publish an image to Docker Hub
   ```
   docker push <username>/<image_name>
   ```

Push Image to Docker Hub
   ```
   docker push <image_name>
   ```

Pull an Image from Docker Hub
   ```
   docker pull <image_name>
   ```

### Docker General Commands

Start Docker Service
   ```
   sudo service docker start
   ```

Stop Docker Service
   ```
   sudo service docker stop
   ```

Restart Docker Service
   ```
   sudo service docker restart
   ```

Show Docker System Information
   ```
   docker info
   ```

Display Docker Disk Usage
   ```
   docker system df
   ```

List Running Containers
   ```
   docker ps
   ```

List All Containers (including stopped)
   ```
   docker ps -a
   ```

Run a Container from an Image
   ```
   docker run <image_name>
   ```

Stop a Running Container
   ```
   docker stop <container_id>
   ```

Remove a Container
   ```
   docker rm <container_id>
   ```

Execute a Command in a Running Container
   ```
   docker exec -it <container_id> <command>
   ```

View resource usage stats
   ```
   docker container stats
   ```

Remember to replace placeholders like `<image_name>` or `<container_id>` with actual names or IDs. Additionally, ensure proper permissions (usually requiring `sudo` for Linux) for Docker commands if necessary.