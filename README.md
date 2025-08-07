# mem0 Docker Build

This project automatically builds and pushes Docker images for the [mem0](https://github.com/mem0/mem0) OpenMemory project.

## How it works

This project uses a GitHub Actions workflow to build and push the `mem0` Docker images to Docker Hub. The workflow is triggered when a new version of `mem0` is released.

The workflow builds two Docker images:

- `mem0-api`: The backend API for the `mem0` application.
- `mem0-ui`: The user interface for the `mem0` application.

## How to use the Docker images

The Docker images are available on Docker Hub:

- `mem0-api`: https://hub.docker.com/r/jkhearsc/mem0-api
- `mem0-ui`: https://hub.docker.com/r/jkhearsc/mem0-ui

To use the Docker images, you can use the `docker-compose.yml` file:
`docker compose up -d`

## Versioning

The Docker images are versioned using the `mem0` release version. For example, if the `mem0` release version is `v0.1.115`, the Docker images will be tagged with `v0.1.115`.

The `latest` tag will always point to the latest release of `mem0`.
