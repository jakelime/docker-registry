# Project Context: Docker Registry UI

## Overview

This repository hosts the infrastructure configuration to deploy
a self hosted solution using docker-compose.

## Tech Stack

- **Containerization**: Docker, Docker Compose
- **Web Server**: Nginx
- **Scripting**: Bash, Python

- Docker images
- Official `registry` image from Docker [docker-hub-url](https://hub.docker.com/_/registry)
- Official `nginx` image from Docker [docker-hub-url](https://hub.docker.com/_/nginx)
- `joxit/docker-registry-ui` image from Docker [docker-hub-url](https://hub.docker.com/r/joxit/docker-registry-ui)
  - This is to build the user interface to manage the docker registry

## Coding Standards & Preferences

1. **Security First**:
   - Always enforce HTTPS.
   - Do not commit secrets or API keys; use environment variables.
   - Prefer strict SSL cipher suites.

1. **Code Style**:
   - **Nginx**: Indent with 2 spaces. Group related directives (e.g., SSL settings) together.
   - **Comments**: Comment complex logic, especially workarounds for specific legacy clients (like old Docker versions).

## Known Constraints

- The Synology environment has specific path mapping requirements. Ensure paths match the mounted volumes.
