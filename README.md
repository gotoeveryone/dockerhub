# dockerhub

## Requirements

- Docker

## Build & Push

```console
$ docker login
$ docker buildx create --name multiplatform --driver docker-container --use
$ docker buildx inspect --bootstrap multiplatform
$ docker buildx build --platform linux/amd64,linux/arm64 -t {account_name}/{image_name}:{version} --push {directory}
$ docker push {account_name}/{image_name}:{version}
```
