[![Circle CI](https://circleci.com/gh/yikaus/docker-alpine-base.svg?style=svg)](https://circleci.com/gh/yikaus/docker-alpine-base)

# Build alpine from source 

Almost same build scripts with [docker-alpine] to  Build docker alpine base image from source by circleci . 

A bit of difference is instead of push docker image directly to docker hub , I choose push root.fs back to this repository .

It could be more clear that docker build still happened in docker hub site and see [yikaus/alpine-base]

You can check version by 
- docker pull yikaus/alpine-base
- docker run --rm yikaus/alpine-base  cat /etc/issue
- docker pull yikaus/alpine-base:2.7
- docker run --rm yikaus/alpine-base:2.7  cat /etc/issue

Why circleci ? because it seems the only build system support running docker in script.

- Travis :    Default CI machine kernel 2.6 does not support docker , it 's docker infrustructure don't support sudo

- Drone.io:   Dosen't support docker privilege  mode .

- Shippable:  Docker in docker not support yet.


[docker-alpine]: https://github.com/gliderlabs/docker-alpine 
[yikaus/alpine-base]: https://registry.hub.docker.com/u/yikaus/alpine-base/
 
