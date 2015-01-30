[![Build Status](https://travis-ci.org/yikaus/docker-alpine-base.svg)](https://travis-ci.org/yikaus/docker-alpine-base)

# Build alpine from source 

Sadly none of those big hostCI support running docker within docker/vm

Travis :    default CI machine kernel 2.6 does not support docker , it 's docker infrustructure don't support sudo
Drone.io:   hosted service dosen't support privilege  mode .
Shippable:  It says docker in docker is coming soon, but still not now (30/01/2015 updated)  
 
