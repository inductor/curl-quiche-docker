# curl-quiche-docker

## How to use

### If you want to try out from DockerHub
```
docker run --rm -it ghcr.io/inductor/curl-quiche
```

### If you want to build the image by yourself
Note: For high-efficient concurrent building, I strongly recommend you to use BuildKit  
Use Docker 18.09.x or later

```
DOCKER_BUILDKIT=1 docker buildx build . -t some/tag
docker run --rm -it some/tag
# curl --http3 https://www.facebook.com/ -v -s -o /dev/null
```
