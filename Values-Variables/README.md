# Storing parameters as environment variables

Here we create an image that can ping any given site, with a `host environment variable`

## Build the docker image:
`docker build -t pinger .`

The Dockerfile has a default value set for the `host`, in case one is not provided

### Run the container with default host:
`docker run --rm pinger`

### With a provided host:
`docker run --rm -e host=www.bing.com pinger`
