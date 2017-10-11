# NPM Mirror 

[![Image Layers](https://images.microbadger.com/badges/image/garethflowers/npm-mirror.svg)](https://microbadger.com/images/garethflowers/npm-mirror)
[![Docker Pulls](https://img.shields.io/docker/pulls/garethflowers/npm-mirror.svg)](https://store.docker.com/community/images/garethflowers/npm-mirror)

A NPM Mirror server, using `sinopia`.

## How to use this image

### Start a NPM Mirror Server instance

To start a container, with data stored in /home/storage on the host, use the
following:
```sh
docker run --name some-npm-mirror-server \
           --detach \
           --volume /home/storage:/var/opt/sinopia \
           --publish 4873:4873 \
           garethflowers/npm-mirror
```

## License

* This image is released under the [MIT License][1]

 [1]: https://raw.githubusercontent.com/garethflowers/npm-mirror/master/LICENSE
