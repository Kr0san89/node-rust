# Docker Node & Rust Image

[![dockeri.co](https://dockerico.blankenship.io/image/krosan89/node-rust)](https://hub.docker.com/r/krosan89/node-rust)

[![GitHub issues](https://img.shields.io/github/issues/Kr0san89/node-rust.svg "GitHub issues")](https://github.com/Kr0san89/node-rust)
[![GitHub stars](https://img.shields.io/github/stars/Kr0san89/node-rust.svg "GitHub stars")](https://github.com/Kr0san89/node-rust)

Having the current stable node docker images with the newest rust see https://github.com/nodejs/docker-node

Package will be built at least once a month with a Github Action to ensure latest security fixes from NodeJS and new Rust versions are provided

Dockerhub Image: https://hub.docker.com/r/krosan89/node-rust

## Build Image Manually
### Node 18
```
docker build --progress plain -t krosan89/node-rust:18 .
docker push krosan89/node-rust:18
```

### Node 20

```
docker build --progress plain -t krosan89/node-rust:20 -t krosan89/node-rust:latest .
docker push krosan89/node-rust:20
```
