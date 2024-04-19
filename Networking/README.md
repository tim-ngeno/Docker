# Networking

The `EXPOSE` instruction is used to document which ports should be redirected to the 'outside' of the image.

For instance, a HTTP server generally listens on the TCP port 80. To make this explicit call in your Dockerfile:
`EXPOSE 80`

Using this instruction is purely for documentation purposes. It will NOT open a port to the outside world when a container is created from that image. Anyone who creates a container will need to explicitly bind that port to an actual port of the host machine using the -p switch of the docker run command.
