---
layout: post
author: dieter_hubau
title: 'Devoxx15: Docker and Kubernates at Google'
---
# Docker & Kubernetes at Google

## Docker
- Open Source
- Container Creation for applications
- Build, Ship, Run
- DockerHub to share docker images (because sharing is caring)
- Docker engine runs on minimal operating system
- Docker app runs on the Docker engine
- This is in contrast with regular VMs, running on full-blown OS

## Docker build (docker CLI)
- Dockerfile defines list of commands to builds image
- Need to set different DOCKER environment variables to determine docker_host etc
- Union File system: Bootfs kernel > Base Image (the chosen OS) > (multiple) images
- All commands are compressed into one, customized docker image for you

## Docker machine (docker-machine CLI)
- docker-machine create --driver=virtualbox myhost
- CLI to configure Docker client,
- creates and pulls images
- start, stop, restart containers
- upgrade Docker itself
- many plugins exist for various cloud providers
- advice: don't use in production (yet!)

## Boot2Docker
- earlier version of docker-machine
- being used by docker-machine in the background
- advice: migrate to docker-machine

## Docker Toolbox
- easiest tool to get started with Docker

## Hands-on Docker
- `docker help`for all your docker needs!
- 