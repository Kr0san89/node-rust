# Docker Node & Rust Image

Having the current stable node docker images with the newest rust

see https://github.com/nodejs/docker-node

## Build Image Manually


### 18
<code>
docker build --progress plain -t krosan89/node-rust:18 .

docker push krosan89/node-rust:18
</code>

### 20

<code>
docker build --progress plain -t krosan89/node-rust:20 -t krosan89/node-rust:latest .

docker push krosan89/node-rust:20
</code>
