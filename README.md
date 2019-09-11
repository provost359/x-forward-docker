# x-forward-docker

Image that forwards the containerized Firefox browser to the host running an X.org server.

Initialize and run with the following (change IP to that of the X.org server):

`docker build -t x-forwarding .`

`set-variable -name DISPLAY -value 192.168.0.110:0.0`

`docker run -ti --rm -e DISPLAY=$DISPLAY x-forwarding`
