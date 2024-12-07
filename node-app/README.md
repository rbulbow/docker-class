# node-app

<!-- TOC -->

- [node-app](#node-app)
- [About](#about)
- [Run this image](#run-this-image)
- [Contributing](#contributing)
  - [Updating this image](#updating-this-image)
  - [Publishing the image](#publishing-the-image)
    - [Option-1](#option-1)
- [License](#license)

<!-- TOC -->

# About

Web application developed node

# Run this image

## In Docker container:

```bash
docker run -d -p 8080:8080 --rm rbow/node-app:1.0.0
```

# Contributing

* See the [REQUIREMENTS.md](REQUIREMENTS.md) file.
* See the [CONTRIBUTING.md](CONTRIBUTING.md) file.

## Updating this image

* Change the ``Dockerfile``.

* Commands to build the image:

```bash
cd node-app

docker build -t rbow/node-app:1.0.0 .
```

## Publishing the image

### Option 1

* Create or access your account in Docker Hub and create the repository for custom image. Example: https://hub.docker.com/r/DOCKER_HUB_ACCOUNT/node-app. 

* Create a git tag and send it to the remote repository. The image will be built for various processor architectures and pushed to Docker Hub.

# License

* See the [LICENSE](LICENSE) file.
