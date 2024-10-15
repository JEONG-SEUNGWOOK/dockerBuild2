# dockerfiles-ubuntu-user-adderable
Ubuntu, It support base user creation and password setting.

# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build   --rm -t jsw7767/ubuntu:test .
	docker run -it --rm --name u1  jsw7767/ubuntu:test
```
Get the port that the container is listening on:

```
# docker ps
CONTAINER ID        IMAGE                COMMAND             CREATED             STATUS              PORTS               NAMES
fc199e02d300        jsw7767/ubuntu:test   "/bin/bash"         41 seconds ago      Up 40 seconds                           u1
```

To test, ("jsw7767" is username. )
```
	tree
```
To Rollback
```
    docker rm u1 -f
    docker rmi jsw7767/ubuntu:test
```
