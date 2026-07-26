# Docker Basics

## Index

1. What Docker is
2. Containers versus virtual machines
3. Images and containers
4. Dockerfile fundamentals
5. Running your first container
6. Docker Hub and registries
7. Volumes and persistent data
8. Docker networking
9. Basic Docker commands
10. Common container lifecycle concepts
11. Troubleshooting basics
12. Why Docker is important in DevOps

## 1. What Docker is

Docker is a platform that packages applications and their dependencies into containers. A container is a lightweight, portable runtime unit that can run consistently across development, testing, and production machines. This makes it easier for teams to share environments and reduce the classic “it works on my machine” problem.

### Subtopics

- Containerization platform
- Portable application packaging
- Standardized runtime environment
- Lightweight alternative to full VMs

## 2. Containers versus virtual machines

Containers are different from virtual machines because they share the host operating system kernel rather than requiring a full guest OS. This makes containers faster to start and lighter on resources. VMs provide stronger isolation, but they are usually heavier and slower. In many modern systems, containers are preferred for application delivery.

### Subtopics

- Shared kernel model
- Faster startup
- Lower overhead
- Better for microservices

## 3. Images and containers

A Docker image is a read-only template used to build a container. A container is a running instance of an image. Images can be built from a Dockerfile, pulled from a registry, or created from another image. Understanding the difference between image and container is central to using Docker well.

### Subtopics

- Image layers
- Container runtime state
- Immutable image model
- Container IDs and names

## 4. Dockerfile fundamentals

A Dockerfile is a text file that contains instructions for building an image. It can define the base image, install dependencies, copy application files, expose ports, and set startup commands. A well-written Dockerfile helps create consistent and repeatable images.

### Subtopics

- FROM instruction
- COPY and ADD
- RUN and CMD
- EXPOSE
- ENTRYPOINT and CMD differences

## 5. Running your first container

You can run a container with a simple command such as launching a web server or an application image. The container starts in the background, exposes a port, and can be stopped or removed as needed. Running containers is the most direct way to understand how Docker behaves in practice.

### Subtopics

- docker run
- Detached mode
- Port mapping
- Container logs
- Stopping and removing containers

## 6. Docker Hub and registries

Docker Hub is the default public registry for many images, but private registries are also common in enterprise environments. Registries store images so they can be shared across systems and teams. Using a registry makes deployments more consistent and prevents teams from building everything manually.

### Subtopics

- Public and private registries
- docker pull and docker push
- Image tags
- Authentication and access control
- Harbor and Azure Container Registry

## 7. Volumes and persistent data

Containers are ephemeral by default, which means data inside them can disappear when the container is removed. Docker volumes solve this by providing persistent storage that survives container replacement. Volumes are essential for databases, logs, and other stateful services.

### Subtopics

- Named volumes
- Bind mounts
- Data persistence
- Backup strategy
- Stateful services

## 8. Docker networking

Docker networking allows containers to communicate with each other and with the outside world. By default, Docker creates bridge networks, but you can also define custom networks. Understanding networking is important for multi-container applications, service discovery, and access control.

### Subtopics

- Bridge network
- Host network
- Container-to-container communication
- Port publishing
- Network isolation

## 9. Basic Docker commands

Docker has a small set of core commands that are used every day. These include commands to build images, list containers, inspect them, attach to them, and remove them. Learning these commands early makes it easier to work with Docker confidently.

### Subtopics

- docker build
- docker ps
- docker images
- docker inspect
- docker logs
- docker rm and docker rmi

## 10. Common container lifecycle concepts

Containers go through a lifecycle that includes creation, running, pausing, stopping, restarting, and removal. Understanding this lifecycle helps you manage services properly, especially in development and deployment pipelines. It also helps you reason about failures and resource consumption.

### Subtopics

- Create and start
- Stop and restart
- Pause and unpause
- Remove containers
- Container health state

## 11. Troubleshooting basics

Docker troubleshooting often involves inspecting logs, checking container status, and reviewing configuration. Common issues include port conflicts, missing files, dependency problems, and memory limits. Learning to diagnose these issues quickly is an important skill in DevOps environments.

### Subtopics

- docker logs
- docker inspect
- Port conflict issues
- Permission issues
- Image build failures

## 12. Why Docker is important in DevOps

Docker is important in DevOps because it makes application deployment more predictable and easier to automate. It helps teams package software once and run it everywhere, which reduces environment drift and speeds up release cycles. Docker also fits naturally into CI/CD pipelines and cloud-native systems.

### Subtopics

- Reproducible environments
- Faster deployment
- Cloud compatibility
- Microservices support
- CI/CD automation
